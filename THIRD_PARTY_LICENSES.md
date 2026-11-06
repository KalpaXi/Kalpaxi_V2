# Third-party licences

KalpaXi is licensed under the **GNU Affero General Public License v3.0** (see `LICENSE`).
It uses or bundles the open-source components below. Each keeps its own licence;
nothing here changes those licences.

> **Maintainers:** before each release, confirm every row against the actual
> dependencies and the versions shipped in the installer. Rows marked *(confirm)*
> are expected but not yet verified. Remove anything KalpaXi does not use.

## Components

| Component | Used for | Licence | Shipped in installer | Source |
|---|---|---|---|---|
| Open CASCADE Technology (OCCT) | Geometry kernel (parts, Booleans, STEP) | LGPL-2.1 with Open CASCADE Exception | Yes *(confirm)* | https://dev.opencascade.org |
| Three.js | 3D viewing in the user interface | MIT | Yes | https://github.com/mrdoob/three.js |
| Gmsh | Meshing (C3D10 tetrahedra) | GPL-2.0-or-later, with Gmsh exceptions | Yes, as a separate program *(confirm)* | https://gmsh.info |
| CalculiX (ccx) | Finite-element solver | GPL-2.0 | Yes, as a separate program *(confirm)* | http://www.calculix.de |
| Python | Local analysis helper | PSF License | Yes *(confirm)* | https://www.python.org |
| NumPy | Numerical calculations | BSD-3-Clause | *(confirm)* | https://numpy.org |
| SciPy | Numerical methods | BSD-3-Clause | *(confirm)* | https://scipy.org |
| pandas | Result tables | BSD-3-Clause | *(confirm)* | https://pandas.pydata.org |
| pyLife | Fatigue calculations | Apache-2.0 | *(confirm)* | https://github.com/boschresearch/pylife |
| Flask | Registration server (not in the desktop installer) | BSD-3-Clause | No | https://flask.palletsprojects.com |

Add rows for any other library found in the project's dependency files
(`package.json`, `requirements.txt` or similar).

## Programs called as separate processes

Gmsh and CalculiX are run as **separate programs**: KalpaXi writes input files,
starts the program and reads its result files. They are not linked into KalpaXi's code.

## Source code for GPL components

Gmsh and CalculiX are licensed under the GPL. When their executables are included
in a KalpaXi installer, the **exact source code of the versions shipped** is made
available with the same release, on the https://github.com/KalpaXi/KalpaXi_V2/releases page, or on request from
admin@kalpaxi.in for at least three years after the release.

## Full licence texts

Full texts of each licence are in the `licenses/` folder of the installer and of
this repository *(maintainers: add one text file per licence before release)*.
