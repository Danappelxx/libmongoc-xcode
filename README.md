# libmongoc-xcode
This repository is a mirror of the [MongoDB C driver](https://github.com/mongodb/mongo-c-driver) library, except the source files are place in an Xcode project. This is done to allow libmongoc to build through Carthage.

# Dependencies
The MongoDB C driver depends on libbson, so because of that, so does this. Carthage takes care of this for us, though.

# Usage
Add the following line to your Cartfile:
```carthage
github "Danappelxx/libmongoc-xcode" "master"
```
and run 
```shell
$ carthage bootstrap
```
in your source file, simply
```swift
import bson
import mongoc
```
and enjoy!

# Documentation
Documentation is available [here](http://api.mongodb.org/c/current/).
