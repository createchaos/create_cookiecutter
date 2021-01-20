# CREATE Lab Package Template

This is a COMPAS-opinionated template that automates the set up of a new
python-based code extension package using
[cookiecutter](https://cookiecutter.readthedocs.io/). We will, little-by-little,
give it our own CREATE Lab twist!

This repository provides you with the basic infrastructure to kickstart your next project: a base folder structure, auto-documentation, testing, pip installing, and easier-integration with Rhino.

## What comes in the box?

* Project directory and file structure
* Documentation based on [Sphinx](http://www.sphinx-doc.org/en/master/)/[reStructuredText](http://docutils.sourceforge.net/rst.html)
* A testing framework: [pytest](https://docs.pytest.org/en/latest/)
* Basic setup script to create pip installable packages
* Automation of common tasks for development workflow based on [pyinvoke](http://www.pyinvoke.org/) (generate documentation, run tests, check format, etc.)
* [EditorConfig](https://editorconfig.org/) integration
* Minimal [Travis-CI integration](https://travis-ci.org)

### What files are automatically created for you?

* `.github`
* `data`
* `docs`
* `docsource`
* `examples`
* `src`
* `temp`
* `tests`

* `.bumpversion.cfg`
* `.editorconfig`
* `.gitignore`
* `.travis.yml`

* `AUTHORS.md`
* `CHANGELOG.md`
* `CONTRIBUTING.md`
* `LICENSE`
* `MANIFEST.in`
* `pytest.ini`
* `README.md`
* `requirements-dev.txt`
* `requirements.txt`
* `setup.cfg`
* `setup.py`
* `tasks.py`

## What do you need to install first?

Install `cookiecutter` command line: `pip install cookiecutter`

## How do I use this thing?

In the terminal or Anaconda prompt, go to the folder where you store all of your projects, (such as "repos", "github" etc.):

```
$ cd <your-projects-folder>
```

Cookiecutter will create a folder for your project and fill it with template files. To instigate this this, run the following command and answer the prompts:

```
$ cookiecutter gh:createchaos/create_cookiecutter
```

To access your new project folder via the command line:

```
$ cd <project-slug>
```

## Advanced features

To activate continuous integration (e.g. you are developing a package that is adequately tested, and every time you want to make an official release, you want to make sure all tests - among other things - are adequately passed).

* [Enable the repository in your Travis CI account](https://travis-ci.org/profile).

## License

This template is forked from the COMPAS'framework [cookiecutter template for COMPAS extensions](https://github.com/compas-dev/tpl-extension), and as such, it
is licensed under the terms of the [MIT License](/LICENSE).
