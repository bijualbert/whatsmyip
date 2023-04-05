# whatsmyip

* This is a simple shell script to get your host public IP (Internet IP) and output the results.   Most free providers of this service limit it's use.   If your scripts poll them too often, you will get blocked.  This script uses a randomly selected provider and will try others if it fails to provide a result.   Also, some providers give the results in XML, JSON or some other format.  This script takes care of that and simply echos your IP.

## Enhancements I would like to do or accepting Pull Requests if you know some scripting
* There are MANY providers around the world that provide this service and I would like to know some of your favorits (and most reliable) to expand my current list.
* Need to add more documentation
* Need to add --help to script
* Move the providers to an array.
* Add new option to validate all providers (thats why I want to have an array of providers)
* Create a Makefile, "make install" and "make uninstall"

## Installation.
* Simply copy this script to a directory in your PATH.
```
$ sudo cp ./whatsmyip /usr/local/bin
```

## Usage
```
$ whatsmyip
60.70.80.90

$ MYIP=$(whatsmyip)
$ echo $MYIP
60.70.80.90
