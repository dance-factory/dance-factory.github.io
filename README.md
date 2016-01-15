# Installation

- [Hugo](https://gohugo.io/overview/installing/)
- Sass: gem install sass (requires ruby)

# Generation

- To generate css from sass: `sass --watch pre-compile/main.sass:static/css/main.css`
- To start hugo server for development: `hugo server`
- To deploy hugo to its public directory: `hugo`

# Branches

Development on dev branch, then push public directory on master:

    git subtree push --prefix public origin master
    
In case of push problems with subtree, force with:

    git push origin `git subtree split --prefix public master`:master --force
