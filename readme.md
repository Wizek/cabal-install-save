This is a shell script 'solution' I've put together so we can have [this](https://github.com/haskell/cabal/issues/1961) functionality even before it is implemented in cabal.

It looks for the latest version of the specified package, adds it to the *.cabal file then does a `cabal install --only-dependencies`.

Installation:

```bash
$ git clone git@github.com:Wizek/cabal-install-save.git
$ # Export to path:
$ echo 'export $PATH:'`pwd`'/cabal-install-save/bin' >> ~/.*hrc
```

Usage: 

```bash
$ cd /to/a/cabal/project
$ cabal-install-save foobar
``` 

Questions, comments, issues and pull requests are welcome.
