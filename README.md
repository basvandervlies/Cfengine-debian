# cfengine-debian
CFengine debian packages

cfengine debian build

    To update the submodules like slurm git submodule foreach --recursive git pull

Build the package

The following steps to build for example 17.11:

    cd core
    git checkout 3.12.x
    ln -s ../debian .
    dch -n (maybe w must upgrade the version number)
    debian/rules build
    fakeroot debian/rules binary
