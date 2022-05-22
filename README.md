# Freifunk Ilmenau - Firmware builds

### How to build the Gluon based Freifunk Ilmenau Firmware
```
# Get the official Gluon repository and switch to a Gluon release
git clone -b v201x.y.z git://github.com/freifunk-gluon/gluon.git
# Get the Freifunk Ilmenau site repository and switch to site config release
git clone -b v201x.y.z https://github.com/freifunk-ilmenau/site-ffil.git gluon/site

cd gluon
# Get other repositories used by Gluon
make update
# Build Gluon for a target
make GLUON_TARGET=target
```

#### Targets

To see a complete list of supported targets, call

    make

without setting GLUON_TARGET.

For further information about supported hardware and targets please see [Supported Devices & Architectures ](http://gluon.readthedocs.io/en/latest/index.html#supported-devices-architectures) in the official Gluon documentation.

#### Example
```
git clone -b v2018.2.2 git://github.com/freifunk-gluon/gluon.git
git clone -b v2018.2.2 https://github.com/freifunk-ilmenau/site-ffil.git gluon/site
cd gluon
make update
make GLUON_TARGET=ar71xx-generic
```

#### Gluon documentation

Please see [the official Gluon documentation](http://gluon.readthedocs.io/en/latest/user/getting_started.html) for a detailed explanation of the build process. You can also consult [the official Gluon repository](https://github.com/freifunk-gluon/gluon) for additional information.

### Gluon releases used for specific Freifunk Ilmenau Firmware builds

- 2018.2.x: v2018.2.x
