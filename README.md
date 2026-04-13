About netgen-feedstock
======================

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/netgen-feedstock/blob/main/LICENSE.txt)

Home: https://ngsolve.org/

Package license: LGPL-2.1-only

Summary: Automatic 3d tetrahedral mesh generator with Python interface

Development: https://github.com/NGSolve/netgen

Documentation: https://ngsolve.org/

NETGEN is an automatic 3d tetrahedral mesh generator with Python interface.
It accepts input from constructive solid geometry (CSG) or boundary representation (BRep)
from STL file format. The connection to a geometry kernel (OCCT) allows the handling
of IGES and STEP files. NETGEN contains modules for mesh optimization and
hierarchical mesh refinement. Open source, LGPL license; available for Linux, macOS and Windows.

Current build status
====================


<table>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-netgen-green.svg)](https://anaconda.org/freecad/netgen) | [![Conda Downloads](https://img.shields.io/conda/dn/freecad/netgen.svg)](https://anaconda.org/freecad/netgen) | [![Conda Version](https://img.shields.io/conda/vn/freecad/netgen.svg)](https://anaconda.org/freecad/netgen) | [![Conda Platforms](https://img.shields.io/conda/pn/freecad/netgen.svg)](https://anaconda.org/freecad/netgen) |

Installing netgen
=================

Installing `netgen` from the `freecad` channel can be achieved by adding `freecad` to your channels with:

```
conda config --add channels freecad
conda config --set channel_priority strict
```

Once the `freecad` channel has been enabled, `netgen` can be installed with `conda`:

```
conda install netgen
```

or with `mamba`:

```
mamba install netgen
```

It is possible to list all of the versions of `netgen` available on your platform with `conda`:

```
conda search netgen --channel freecad
```

or with `mamba`:

```
mamba search netgen --channel freecad
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search netgen --channel freecad

# List packages depending on `netgen`:
mamba repoquery whoneeds netgen --channel freecad

# List dependencies of `netgen`:
mamba repoquery depends netgen --channel freecad
```




Updating netgen-feedstock
=========================

If you would like to improve the netgen recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`freecad` channel, whereupon the built conda packages will be available for
everybody to install and use from the `freecad` channel.
Note that all branches in the conda-forge/netgen-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks, and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@looooo](https://github.com/looooo/)

