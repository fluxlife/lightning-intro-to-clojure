# Intro to Clojure

This is a barebones clojure project with a Juptyer Notebook that goes through
the basics of Clojure. All of the material is in the 
[Jupyter notebook](Learning-Clojure.ipynb).

# How to get started
## Install Clojure
- Follow guide [here](https://clojure.org/guides/getting_started)

### TLDR
#### Mac 
```
brew install clojure
```
#### Linux
```
$ curl -O https://download.clojure.org/install/linux-install-1.10.0.414.sh
$ chmod +x linux-install-1.10.0.414.sh
$ sudo ./linux-install-1.10.0.414.sh
```
#### Windows
see `Install Leiningen` below

## Install leiningen

### Wait ... Why?
- It's essentially a Clojure build tool. 
- Leiningen is to Clojure as
  - Maven/Gradle is to Java
  - SBT is to Scala
  - etc
- Technically, you don't need it. 
  - You can do all of your package management and building with the clojure cli tools
    - Guide [Here](https://clojure.org/guides/deps_and_cli)
  - But for convenience and online examples you'll look at, you should use it for now.
  - If you want to utilize the notebook in this repo, you will need leiningen

#### Mac
```
brew install leiningen
```

#### Everyone else
[Install Leiningen](https://leiningen.org/#install) from instructions

  
## To follow along ...
- Do the above then ...

### In a Terminal
```
$ clj
```
  - Opens a REPL and you can start experimenting

### In a notebook
- clone this repo
- install juptyer (if you haven't already)
```
$ python3 -m pip install --upgrade pip
$ python3 -m pip install jupyter
```
- run: 
```
$ lein jupyter install-kernel
```
- finally: 
```
$ lein jupyter notebook
```

## Quick note about Juptyer Notebook & Clojure
If you evaluate anything in the notebook that returns 'null',
it will crash the kernel and you will need to restart the kernel.
You can do this from the Notebook by going to the `Kernel` menu
and selecting `Restart`