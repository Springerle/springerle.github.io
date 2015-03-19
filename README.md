# ![❏](https://raw.github.com/Springerle/springerle.github.io/master/static/img/logo-64.png) Springerle

This is the website for “Springerle” ([/ʃpʀɪŋɛʀlə/](https://translate.google.com/#de/de/Springerle)),
a collection of cookiecutter molds mostly for Python and Java.

## Motivation and Goals

The main goal of *Springerle* is to provide basic templates and add-on facets to incrementally set up projects in a flexible and composable manner.

See “[Using the templates](#using-the-templates)” for details on which templates are available,
and the following section for pre-requisites.


## Installing the cookiecutter CLI

The following is an easy way to install the `cookiecutter` command line tool into your `$HOME`,
with the help of [pipsi](https://github.com/mitsuhiko/pipsi).

```sh
# add "pipsi" bin dir to PATH, permanently
grep '/.local/bin:' ~/.bash_aliases >/dev/null 2>&1 || echo >>~/.bash_aliases \
    'grep ":$HOME/.local/bin:" <<<":$PATH:" >/dev/null || export PATH="$HOME/.local/bin:$PATH"'
source ~/.bash_aliases

# possibly activate a HTTP proxy or PyPI mirror here, if you're firewalled

# install "pipsi" and "cookiecutter"
which pipsi || curl "https://raw.githubusercontent.com/mitsuhiko/pipsi/master/get-pipsi.py" | python
which cookiecutter || pipsi install cookiecutter
cookiecutter --version
```
:bulb: | If you later want to update to a new version, just issue a `pipsi upgrade cookiecutter` command and you're done.
---- | :----


## Using the templates

The Springerle [cookie-jar](https://github.com/Springerle/cookie-jar) repository collects pointers
to ‘releases’ of the templates, i.e. references to tags in the various subprojects.
These take the form of git submodules, so that you can check out all the templates in one fell swoop,
and use them off-line or package them in some form.

:bulb: | To get *your* defaults for common template values `cookiecutter` will ask you for when you use a template, it makes sense to have a [~/.cookiecutterrc](https://github.com/jhermann/ruby-slippers/blob/master/home/.cookiecutterrc) in your home directory. Follow the link to see an example.
---- | :----


## Addendum

![CC0 license](http://img.shields.io/badge/license-CC0-red.svg)  *for this page (README).*

[![1&1](https://raw.githubusercontent.com/1and1/1and1.github.io/master/images/1and1-logo-42.png)](https://github.com/1and1)  Project sponsored by [1&1](https://github.com/1and1).
