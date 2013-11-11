# sprout-wrap

[![Build Status](https://travis-ci.org/pivotal-sprout/sprout-wrap.png?branch=master)](https://travis-ci.org/pivotal-sprout/sprout-wrap)

This project uses [soloist](https://github.com/mkocher/soloist) and [librarian-chef](https://github.com/applicationsonline/librarian-chef)
to run a subset of the recipes in sprout's [cookbooks]((https://github.com/pivotal-sprout/sprout).

## Installation

```
$ git clone https://github.com/wireframe/sprout-wrap.git
$ cd sprout-wrap
$ bin/provision
```

## Updating

The `bin/provision` script will automatically update your local configuration and re-run soloist to install/update any new recipes.

## Local Customization

customize attributes and add new recipes using `~/.soloistrc_local` file.

example:

```yaml
# example to add new recipes
recipes:
- applications::evernote

# example to customize/override node attributes
node_attributes:
  git:
    email: someone@acompany.com
```
