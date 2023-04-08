# Dharmesh's Recipe Library

This repository is a collection of recipes I want to file away in a searchable/taggable way.

## Dependencies:

* [`hugo`](https://gohugo.io/) - converts the pages in the `content` folder into a working website.
* [`paper-mod`](https://github.com/adityatelange/hugo-PaperMod) - the theme used by hugo. It is referrenced via a `git submodule` under `./themes`.
* GitHub Actions - to build the branch, and push it to the `gh-pages` branch.
* GitHub Pages - to host the static website. The site served is from the `gh-pages` branch.

## To contribute:

### Before you start, we recommend

* You have some familiarity with `git`. Specifically how to clone, checkout, push, pull and commit code.
* A copy of `hugo`. Although it is not required, it will allow you to test your changes locally before pushing.
* A text editor to contribute and edit markdown files.

### Steps

#### Checking out and building locally

```
## Clone the repository
git clone https://github.com/dharmeshgordhan/recipelibrary.git
## Clone the git submodule
git submodule update --init --recursive
## Run a dev server locally
hugo server -D
```

#### Contributing a change

1. create a branch
2. create a new page with `hugo new recipe/{recipe-file-name}.md`
3. input your recipe as markdown
4. use the shortcode `{{<c>}}` to add a checkbox in front of each ingredients list item
5. add relevant tags
6. test your build works: `hugo server -D`
7. commit
8. push your code change
9. raise a pull request
10. it'll automatically build and deploy to the `gh-pages` branch when merged via GitHub action