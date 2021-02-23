# Dharmesh Recipe Library

Contains a collection of recipes I want to file away in a searchable/taggable way.

Dependancies (to build and test locally):
* [`hugo`](https://gohugo.io/)

To contribute:
* create a branch
* `hugo new recipe/{recipe-file-name}.md`
* input your recipe as markdown
* use the shortcode `{{<c>}}` to add a checkbox
* add tags
* test your build works: `hugo server -D`
* commit
* raise a PR
* it'll automatically build and deploy to the `gh-pages` branch when merged via GitHub actions
