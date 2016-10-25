# Staging ground for GNSS-SDR snaps

## Building a snap

Install ```snapcraft``` (available on Ubuntu 16.04 LTS and above):

```
$ sudo apt install snapcraft
```

Pick one of the directories, each contains a snapcraft project file:

```
$ cd <directory>
```

Simply type ```snapcraft``` to download all of the dependencies and to build the snap:

```
$ snapcraft
```

The output is a ```.snap``` file.

```
$ ls *.snap
```

## Install a snap

This is an unsigned package, so use ```--force-dangerous```

```
sudo snap install --force-dangerous <package-name>.snap
```

This installs the ```.snap``` file that we just built with snapcraft.
The snap will be unpacked into ```/snap/<package-name>/current```.
Any executables in the snap will be available in the ```$PATH```
and in the ```/snap/bin``` directory as ``<package-name>.<executable-name>``


## Remove a snap

```
sudo snap remove <package-name>
```

## Documentation

* snapcraft yaml syntax: https://developer.ubuntu.com/en/snappy/build-apps/snapcraft-syntax/
* and more on parts: https://developer.ubuntu.com/en/snappy/build-apps/snapcraft-parts/
* app/plugs that allow permissions through apparmor: http://snapcraft.io/docs/reference/interfaces
