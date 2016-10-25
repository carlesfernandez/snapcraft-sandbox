# GNSS-SDR snap


This project creates a working snap of the current 'next' branch of GNSS-SDR.

## How to build the package

Just go to this directory and type:

```
$ snapcraft
```


## How to install the snap package from the Ubuntu Store

* [Install snapd](http://snapcraft.io/docs/core/install)
* ```$ sudo snap install gnss-sdr-next```

You can start using GNSS-SDR like this:

```
$ snap run gnss-sdr-next.volk-gnsssdr-profile
$ snap run gnss-sdr-next.gnss-sdr --config_file=./my_gnss_receiver.conf
```
