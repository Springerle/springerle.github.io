# ![❏](https://raw.github.com/Springerle/springerle.github.io/master/static/img/logo-64.png) Springerle

This is the website for “Springerle” ([/ʃpʀɪŋɛʀlə/](https://translate.google.com/#de/de/Springerle)),
a collection of cookiecutter molds mostly for Python, Java, and technical docs (manuals and presentations).

## Motivation and Goals

The main goal of *Springerle* is to provide basic templates and add-on facets to incrementally set up projects in a flexible and composable manner.

See “[Using the templates](#using-the-templates)” for details on which templates are available,
and the following section for pre-requisites.
To talk about the templates contained in the project, and to get support, please use the
[springerle-users](https://groups.google.com/d/forum/springerle-users)
Google group / mailing list. Please note that only members can post, but anyone can join.


## Installing the cookiecutter CLI

The following installs the `cookiecutter` command line tool into your `$HOME`,
in a dedicated directory you can easily get rid of.

```sh
# possibly activate a HTTP proxy or PyPI mirror here, if you're firewalled

# install "cookiecutter" to its own virtualenv
mkdir -p ~/bin ~/.local/venvs
test -d ~/.local/venvs/cookiecutter \
    || virtualenv ~/.local/venvs/cookiecutter
~/.local/venvs/cookiecutter/bin/pip install -U pip setuptools wheel
~/.local/venvs/cookiecutter/bin/pip install -U cookiecutter
ln -s ~/.local/venvs/cookiecutter/bin/cookiecutter ~/bin
cookiecutter --version
```

To change this to the *patched version* which supports license post-processing
and easy upgrading of existing projects, also run this:

```sh
~/.local/venvs/cookiecutter/bin/pip install -U \
    https://github.com/jhermann/cookiecutter/archive/master.zip
```


## Using the templates

The Springerle [cookie-jar](https://github.com/Springerle/cookie-jar) repository collects pointers
to ‘releases’ of the templates, i.e. references to tags in the various subprojects.
These take the form of git submodules, so that you can check out all the templates in one fell swoop,
and use them off-line or package them in some form.

:bulb: | To get *your* defaults for common template values `cookiecutter` will ask you for when you use a template, it makes sense to have a [~/.cookiecutterrc](https://github.com/jhermann/ruby-slippers/blob/master/home/.cookiecutterrc) in your home directory. Follow the link to see an example.
---- | :----

## Add-on Tools

This is a list of tools that provide additional features to work with Cookiecutter projects and their instances.

 * [senseyeio/cupper](https://github.com/senseyeio/cupper): Update cookiecutter projects using ``git`` and a JSON namespace.
 * [ionelmc/python-cookiepatcher](https://github.com/ionelmc/python-cookiepatcher): Just a small shim around Cookiecutter that alters the CLI a bit, for reapplying templates to existing projects with less headaches.
* [hirokiky/cookiepatcher](https://github.com/hirokiky/cookiepatcher): Tool that applies updates of Cookiecutter templates to projects.
* [cjolowicz/retrocookie](https://github.com/cjolowicz/retrocookie): Updates Cookiecutter templates with changes from generated projects (i.e. the inverse of the cookiepatchers).


## Project Archetype Tools

 * [Cookiecutter](https://github.com/audreyr/cookiecutter): A command-line utility that creates projects from cookiecutters (project templates).
 * [PizzaCutter](https://github.com/bitranox/PizzaCutter): A command-line utility that creates and updates software projects in any language from PizzaCutter project templates. It is conceptually similar to Cookiecutter, but on steroids.

 * [Yeoman](http://yeoman.io/): The web's scaffolding tool for modern webapps.


## Addendum

![CC0 license](http://img.shields.io/badge/license-CC0-red.svg)  *for this page (README).*

[![1&1](https://raw.githubusercontent.com/1and1/1and1.github.io/master/images/1and1-logo-42.png)](https://github.com/1and1)  Project sponsored by [1&1](https://github.com/1and1).
