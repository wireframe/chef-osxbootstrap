# chef-osxbootstrap

This project uses [soloist](https://github.com/mkocher/soloist) and [librarian-chef](https://github.com/applicationsonline/librarian-chef)
to run a configurable set of the Chef recipes for automating installation and configuration of your OSX machine.

## Installation

```
$ git clone https://github.com/wireframe/chef-osxbootstrap.git
$ cd sprout-wrap
$ bin/provision
```

## Updating

The `bin/provision` script will automatically update your local configuration and re-run soloist to install/update any new recipes.

## Local Customizations

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
