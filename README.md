# fedoramy.github.io

## Set up dev env
I use virtualenv is a tool to create isolated Python environments.
```
$ pip install virtualenv
```

fork this repo and navigate into it and run
```
$ python -m venv env
```
it will create a virtual environment for you

To begin using the virtual environment, it needs to be activated:
```
$ source venv/bin/activate
```

Now install the package dependencies.
```
$ pip install -r requirements.txt
```

### Set up sphinx (example)
```
$ sphinx-quickstart
Welcome to the Sphinx 3.3.1 quickstart utility.

Please enter values for the following settings (just press Enter to
accept a default value, if one is given in brackets).

Selected root path: .

You have two options for placing the build directory for Sphinx output.
Either, you use a directory "_build" within the root path, or you separate
"source" and "build" directories within the root path.
> Separate source and build directories (y/n) [n]: y

The project name will occur in several places in the built documentation.
> Project name: Fedora Malaysia
> Author name(s): Robbi Nespu
> Project release []: 1.0.0

If the documents are to be written in a language other than English,
you can select a language here by its language code. Sphinx will then
translate text that it generates into that language.

For a list of supported codes, see
https://www.sphinx-doc.org/en/master/usage/configuration.html#confval-language.
> Project language [en]:

Creating file /home/robbi/Documents/workspace/python/fedoramy.github.io/source/conf.py.
Creating file /home/robbi/Documents/workspace/python/fedoramy.github.io/source/index.rst.
Creating file /home/robbi/Documents/workspace/python/fedoramy.github.io/Makefile.
Creating file /home/robbi/Documents/workspace/python/fedoramy.github.io/make.bat.

Finished: An initial directory structure has been created.

You should now populate your master file /home/robbi/Documents/workspace/python/fedoramy.github.io/source/index.rst and create other documentation
source files. Use the Makefile to build the docs, like so:
   make builder
where "builder" is one of the supported builders, e.g. html, latex or linkcheck.
```

### set up ablog (example)
```
]$ ablog start
Welcome to the ABlog 0.10.12 quick start utility.

Please enter values for the following settings (just press Enter to accept a
default value, if one is given in brackets).

Enter the root path for your blog project (path has to exist).
> Root path for your project (path has to exist) [.]:

Project name will occur in several places in the website, including blog archive
pages and atom feeds. Later, you can set separate names for different parts of
the website in configuration file.
> Project name: Fedora Malaysia
This of author as the copyright holder of the content. If your blog has multiple
authors, you might want to enter a team name here. Later, you can specify
individual authors using `blog_authors` configuration option.
> Author name(s): Robbi Nespu

Please enter the base URL for your project. Blog feeds will be generated
relative to this URL. If you don't have one yet, you can set it in configuration
file later.
> Base URL for your project:

Creating file ./conf.py.
Creating file ./index.rst.
Creating file ./about.rst.
Creating file ./first-post.rst.
Finished: An initial directory structure has been created.
```

## build
you can just run `make html` to build up the static website
```
$ make html
Running Sphinx v3.3.1
loading translations [en]... done
loading pickled environment... failed
failed: build environment version not current
building [mo]: targets for 0 po files that are out of date
building [html]: targets for 3 source files that are out of date
updating environment: [new config] 3 added, 0 changed, 0 removed
reading sources... [100%] index
looking for now-outdated files... none found
pickling environment... done
checking consistency... done
preparing documents... done
writing output... [100%] index
generating indices... genindex done
writing additional pages... search done
copying static files... done
copying extra files... done
dumping search index in English (code: en)... done
dumping object inventory... done
build succeeded.
```
