# GNSS-SDR snap


This project creates a working snap of the current 'next' branch of GNSS-SDR.

## How to build the package

Install snapcraft (available on Ubuntu 16.04 LTS and above):

```
$ sudo apt install snapcraft
```

Then , just go to this directory and type:

```
$ snapcraft
```


## How to install the snap package from the Ubuntu Store

A snap package can be installed in a wide range of Linux distributions, such as Arch Linux, CentOS, Debian, Fedora, Gentoo Linux, OpenSuse, OpenWrt, Red Hat Enterprise Linux and Yocto/OpenEmbedded. In any of those distributions:

* [Install snapd](http://snapcraft.io/docs/core/install)
* ```$ sudo snap install gnss-sdr-next```

You can start using GNSS-SDR like this:

```
$ snap run gnss-sdr-next.volk-gnsssdr-profile
$ snap run gnss-sdr-next.gnss-sdr --config_file=./my_gnss_receiver.conf
```
