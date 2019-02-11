<!--
# -*- mode: jinja -*-
-->

About canmatrix
===============

Home: https://github.com/ebroecker/canmatrix

Package license: BSD-2-Clause

Feedstock license: BSD 3-Clause

Summary: Converting Can (Controller Area Network) Database Formats .arxml .dbc .dbf .kcd ... 

Canmatrix implements a "Python Can Matrix Object" which describes the can-communication and the needed objects (Boardunits, Frames, Signals, Values, ...)
Canmatrix also includes two Tools (canconvert and cancompare) for converting and comparing CAN databases.

There are several importers (read) and exporters (write) for this object.

supported file formats for import:

    .dbc candb / Vector
    .dbf Busmaster (open source!)
    .kcd kayak (open source!)
    .arxml autosar system description
    .yaml dump of the python object
    .xls(x) excel xls-import, works with .xls-file generated by this lib
    .sym peak pcan can description

supported file formats for export:

    .dbc
    .dbf
    .kcd
    .xls(x)
    .json Canard (open source!)
    .arxml (very basic implementation)
    .yaml (dump of the python object)
    .sym
    .xml fibex


Current build status
====================

All platforms:
[![noarch](https://img.shields.io/circleci/project/github/conda-forge/canmatrix-feedstock/master.svg?label=noarch)](https://circleci.com/gh/conda-forge/canmatrix-feedstock)

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-canmatrix-green.svg)](https://anaconda.org/conda-forge/canmatrix) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/canmatrix.svg)](https://anaconda.org/conda-forge/canmatrix) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/canmatrix.svg)](https://anaconda.org/conda-forge/canmatrix) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/canmatrix.svg)](https://anaconda.org/conda-forge/canmatrix) |

Installing canmatrix
====================

Installing `canmatrix` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
```

Once the `conda-forge` channel has been enabled, `canmatrix` can be installed with:

```
conda install canmatrix
```

It is possible to list all of the versions of `canmatrix` available on your platform with:

```
conda search canmatrix --channel conda-forge
```


About conda-forge
=================

[![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-NumFOCUS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](http://numfocus.org)

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](https://www.appveyor.com/)
and [TravisCI](https://travis-ci.org/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](https://anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](https://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating canmatrix-feedstock
============================

If you would like to improve the canmatrix recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/canmatrix-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://conda.io/docs/user-guide/tasks/build-packages/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@altendky](https://github.com/altendky/)
* [@danielhrisca](https://github.com/danielhrisca/)
* [@ebroecker](https://github.com/ebroecker/)

