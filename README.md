# ![❏](https://raw.github.com/Springerle/springerle.github.io/master/static/img/logo-64.png) Springerle

This is the website for “Springerle” ([/ʃpʀɪŋɛʀlə/](https://translate.google.com/#de/de/Springerle)),
a collection of cookiecutter molds mostly for Python and Java.

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
which pipsi || curl https://raw.githubusercontent.com/mitsuhiko/pipsi/master/get-pipsi.py | python
which cookiecutter || pipsi install cookiecutter
cookiecutter --version
```


## Using the templates

**TODO**


## Addendum

![CC0 license](http://img.shields.io/badge/license-CC0-red.svg)  *for the website contents.*

[![1&1](https://raw.githubusercontent.com/1and1/1and1.github.io/master/images/1and1-logo-42.png)](https://github.com/1and1)  Project sponsored by [1&1](https://github.com/1and1).
