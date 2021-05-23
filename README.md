# joshuakasyoka

## Notes to self
## Remember how to push to github
1. Use `git status` to see files that haven't been committed yet
2. Use `git add .` to add all file changes, or `git add FILENAME` to save a specific file
3. Use `git commit -m MESSAGE` to commit the changes to the branch with a message explaining what the changes are
4. Use `git push` to push the changes to remote github
5. Check at `https://joshuakasyoka.github.io/joshuakasyoka/index.html` after a few mins to see if changes have gone through


## CSS Rules
1. Use classes for style that you're going to use again.
`class = "my_class"` and then in the css you reference this by doing `.my_class {}`

2. Use IDs for style that only apply to one thing (i.e - your logo in the header bar)
`id="my_id"` and then in the css you refernce with a `#my_id {}`

3. For styles that apply to all pages, i.e - global font, global colours etc - put in the `globals.css` file. For styles that apply only to a specific page - i.e - `class="blog_heading"` put in the `style.css` file within the relevant folder -> i.e  - the blog folder for this example.