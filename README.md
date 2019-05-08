# cfengine-debian
CFengine debian packages

First clone:
 * `git submodule update --init --recursive`

To update the submodules:
 * `git submodule foreach --recursive git pull`

Build the debian package
 * cd cfengine
 * git checkout 3.12.x
 * ln -s ../debian .
 * dch -n (maybe w must upgrade the version number)
 * debian/rules build
 * fakeroot debian/rules binary
