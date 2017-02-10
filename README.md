# Vimperator organization page

Organization page of vimperator.

The markdown files will be converted to HTML by github pages (using jekyll).

Frequently used links are stored in `_data/links.yml`.
The top menu is created in `_includes/menu.html`.

## Development Setup

Run `gem install jekyll bundler` to install the required ruby gems.
Then clone the repository and change into the directory.
Run `bundle install` to install the requirements from the Gemfile.

To see the current state, run `bundle exec jekyll serve`,
it will run a local server that you can access from a browser.
`jekyll serve` will automatically re-generate the pages when it detects any
changes.
