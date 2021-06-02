# joshuakasyoka

## About 
This is my application for Founders and Coders 
To access this webpage go to `https://joshuakasyoka.github.io/joshuakasyoka/src/entry_page/index.html`

## This website

### Structure

Website
* assets (holds all global images used throughout whole website)
* src
    * a_webpage_folder
        * assets (holds all images for this webpage)
        * webpage.html (the html structure for this webpage)
        * style.css (the style for this webpage)
* global.css (the style for any global classes or ids)
* style.css (TODO: need to merge into global)

### Key F&C Requirements

#### Basic
- [x] All code is written by you
- [x] No external libraries (e.g. no Bootstrap, React or GitHub Pages themes, but external fonts/icons are fine)
- [x] Tells us about why you are applying for the programme
- [x] Hosted on GitHub Pages
- [x] Links back to the GitHub repository that contains the code for your site
- [x] Links to your public freeCodeCamp profile
- [x] Links to your Codewars profile

Additional
- [x] Links to illustration portfolio

#### Technical criteria 
[x] **Semantic HTML5 elements**
Site uses semantic HTML throughout, mostly <nav>, <header>, <section> and <article>

[x] CSS grid or flexbox layout (or both)
**Uses flexbox as this is what I've learned online to use and makes most sense to me**

[x] DOM event listeners for user interaction (e.g. click, keydown)

**On my articles page added 'next' and 'back' buttons**
- This me to get from an array of objects the details to render on the webpage. This keeps the html code clean as I add more information to my page, and makes it easier to maintain (and demonstrate to F&C that I can use javascript in the website). *adapted from various online tutorials*
- JSON -> create a Javascript Object called `articleData` which stores the source for each image `articleData[i].src` and the heading and text.
- JS -> all JS is basic js using `document.getElementById` or `setAttribute` or `style.`
- - 1. When website loads, call `populateSlide()` which fetches the first object (i.e - slideId is 0) and changes the elements to add the src, heading and text.
- - 2. When click 'next', increment slideId and then call populate slide to get the next slide
- - 3. when click 'back', decrease slideId by 1, then call populate slide to get the previous slide.
- - 4. To avoid going to negative index, or above the length of the list, hide 'back' when on `slideId = 0` and hide 'next' when on `slideId = articleData.length-1`


[x] DOM updates in response to user interaction (e.g. showing/hiding an element, changing text or styles)

**On the entry page allow the user to change the theme**
- This changes the background colour, text colour and header colour using css variables
- CSS -> uses css variables and themed based upon guide on W3 Schools: https://www.w3schools.com/css/css3_variables.asp
- CSS Toggle - uses slider from W3 schools: https://www.w3schools.com/howto/howto_css_switch.asp
- JS -> Adapted from this medium blog post: https://medium.com/@haxzie/dark-and-light-theme-switcher-using-css-variables-and-pure-javascript-zocada-dd0059d72fa2
- JS -> Simplified the code from the primary page to add to other pages, which retrieves the theme from local-storage and adds the relevant class!