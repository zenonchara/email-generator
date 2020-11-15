# System Email Dev Harness

## Installation
1. Have Node and NPM, ideally with version at least 10
2. Install dependencies `npm install`

## Usage
1. launch the dev server `gulp watch`. It should open a browser at localhost:3000 or similar
2. You should see a page with a navigation list on the left and email preview in the center
3. use the nav to jump between templates. the compiled HTML of the output will appear on the right
4. copy the right-hand-side content into wherever your system emails live

## To make a new email
1. Make a new html file in `src/templates`
2. To add the new template to the nav list, re-generate the table-of-contents with `gulp toc`
3. Using the existing templates, write your email html code
4. Use CSS classes and html partials to keep your code clean. The gulp task compiles these into useful email code automatically.
5. See your compiled emails in `dist/compiled`

## FAQ

**What aboout the wrapper "base" email?**
Its in `src/templates/_BaseEmailTemplate.html`

**The commands don't seem to be working?**
Check the error console and `package.json` for any missing packages

**The commands don't seem to be working?**
Check the error console and `package.json` for any missing packages
