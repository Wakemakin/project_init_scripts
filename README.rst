project_init_scripts
====================

A set of scripts for all git projects. Provides safety hooks and and virtualenv
creation support.

Installation
------------

Simply download the zip of this repository and place it into your project's
repo. Add created files to git and you should be set!

Usage
-----

This uses rake (make for Ruby) as the driver for the features. It supports the
following tasks:

- rake init: will move the git hooks into the .git directory
- rake makevenv: will create a virtualenv (useful for python developers)

Git Hooks
=========

This will install git hooks that do the following things:

- Pre-commit:

  - Prevents a developer from committing to master branch and promotes the use
    of the pull-request system
