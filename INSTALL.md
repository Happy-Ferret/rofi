# Installation guide:

## DEPENDENCY

### For building:

* C compiler (gcc or clang)
* make
* autoconf
* automake

### External libraries

* libxinerama
* libxft
* libx11
* libxdg-basedir

### Optional:

* For i3 support, you need at least i3 version 4.5 or up.



Install from a release
----------------------

Check dependencies and configure build system:

```
./configure
```

Build Rofi:

```
make
```

The actual install, execute as root (if needed):

```
make install
```


Install a checkout from git
---------------------------

Generate build system:

```
autoreconf -i
```

Create a build directory:

```
mkdir build
```

Check dependencies and configure build system:

```
../configure
```

Build rofi:

```
make
```

The actual install, execute as root (if needed):

```
make install
```


Options for configure
---------------------

When you run the configure step there are several you can configure. (To see the full list type
`./configure --help` ).

The most useful one to set the installation prefix:

```
./configure --prefix=<installation path>
```

f.e.

```
./configure --prefix=/usr/
```

or to install locally:

```
./configure --prefix=${HOME}/.local/
```
