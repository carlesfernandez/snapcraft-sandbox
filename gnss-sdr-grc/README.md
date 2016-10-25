# GNSS-SDR-GRC snap


This project creates a working snap of the current 'next' branch of GNSS-SDR, plus GNU Radio Companion.

It builds from source Volk, a minimal number of GNU Radio libraries and gr-osmosdr.

## How to build the package

Install snapcraft (available on Ubuntu 16.04 LTS and above):

```
$ sudo apt install snapcraft
```

Then, just go to this directory and type:

```
$ snapcraft
```


## How to install the snap

A snap package can be installed in a wide range of Linux distributions, such as Arch Linux, CentOS, Debian, Fedora, Gentoo Linux, OpenSuse, OpenWrt, Red Hat Enterprise Linux and Yocto/OpenEmbedded. In any of those distributions:

* [Install snapd](http://snapcraft.io/docs/core/install)
* ```$ sudo snap install gnss-sdr-grc_0.0.8_*.snap --force-dangerous```

You can start using the snap like this:

```
$ snap run gnss-sdr-grc.volk-gnsssdr-profile
$ snap run gnss-sdr-grc.volk-profile
$ snap run gnss-sdr-grc.gnss-sdr --config_file=./my_gnss_receiver.conf
$ snap run gnss-sdr-grc.gnuradio-companion
```
