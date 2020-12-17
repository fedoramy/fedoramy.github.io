# fedoramy.github.io

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
Note : You can check build files inside `../build/html`


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
$ source env/bin/activate
```

Now install the package dependencies.
```
$ pip install -r requirements.txt
```


