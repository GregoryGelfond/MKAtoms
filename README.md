# MKAtoms

A simple post processor for clingo (and compatible ASP solvers). Originally written by [Marcello Balduccini](https://mbal.asklab.net/) (with the original version available for download [here](https://mbal.asklab.net/mkatoms/), this version is intended to be an easily accessible "fork" for continued developemnt.

## Description

This utility is designed to reformat the output of smodels, in order to put one atom per line. Additionally, it strips off all statistics. Models are separated by a line containing the word `::endmodel`.

## Installation

Simply download the source package, uncompress and untar it, then execute:

```
$ cd MKAtoms
$ ./configure
$ make all
$ make install
```

This will install `mkatoms`, `getone` and `getall` in `/usr/local/bin`. If you want to select a different location, specify a different prefix when you run "configure" as follows:

```
$ ./configure --prefix=/path/where/you/want/MKAtoms/installed
```

Note that you will probably need root access to the system in order to install in `/usr/local/bin`.

## Deprecation Notice

The scripts `getone` and `getall` should be considered deprecated (as lparse and smodels are no longer really utilized). They have not been removed from the installation however to preserve the original version of the utility.
