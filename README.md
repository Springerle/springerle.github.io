# ![❏](https://raw.github.com/Springerle/springerle.github.io/master/static/img/logo-64.png) Springerle

This is the website for “Springerle” ([/ʃpʀɪŋɛʀlə/](https://translate.google.com/#de/de/Springerle)),
a collection of cookiecutter molds mostly for Python and Java.

## Motivation and Goals

The main goal of *Springerle* is to provide basic templates and add-on facets to incrementally set up projects in a flexible and composable manner.

See “[Using the templates](#using-the-templates)” for details on which templates are available,
and the following section for pre-requisites.
To talk about the templates contained in the project, and to get support, please use the
[springerle-users](https://groups.google.com/d/forum/springerle-users)
Google group / mailing list. Please note that only members can post, but anyone can join.


## Installing the cookiecutter CLI

If you are on a 64bit Linux machine, use the *PEX release* as follows:

```sh
curl -Lo ~/bin/cookiecutter \
    "https://github.com/jhermann/cookiecutter/releases/download/v1.0.1/cookiecutter-1.0.1-cp27-none-linux_x86_64.pex"
chmod a+x ~/bin/cookiecutter
cookiecutter --version
```

On other platforms, the following is an easy way to install the `cookiecutter` command line tool into your `$HOME`,
with the help of [pipsi](https://github.com/mitsuhiko/pipsi).

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

To change this to the patched version which supports license post-processing
and easy upgrading of existing projects, also run this:

```sh
~/.local/venvs/cookiecutter/bin/pip install -U \
    https://github.com/jhermann/cookiecutter/archive/master.zip
```

:bulb: | If you later want to update to a new official release version, just issue a `pipsi upgrade cookiecutter` command and you're done.
---- | :----


## Using the templates

The Springerle [cookie-jar](https://github.com/Springerle/cookie-jar) repository collects pointers
to ‘releases’ of the templates, i.e. references to tags in the various subprojects.
These take the form of git submodules, so that you can check out all the templates in one fell swoop,
and use them off-line or package them in some form.

:bulb: | To get *your* defaults for common template values `cookiecutter` will ask you for when you use a template, it makes sense to have a [~/.cookiecutterrc](https://github.com/jhermann/ruby-slippers/blob/master/home/.cookiecutterrc) in your home directory. Follow the link to see an example.
---- | :----

## Project Archetype Tools

 * [Cookiecutter](https://github.com/audreyr/cookiecutter)

 * [Yeoman](http://yeoman.io/) – The web's scaffolding tool for modern webapps.


## Addendum

![CC0 license](http://img.shields.io/badge/license-CC0-red.svg)  *for this page (README).*

[![1&1](https://raw.githubusercontent.com/1and1/1and1.github.io/master/images/1and1-logo-42.png)](https://github.com/1and1)  Project sponsored by [1&1](https://github.com/1and1).
