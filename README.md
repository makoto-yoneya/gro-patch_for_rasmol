# gro-patch_for_rasmol

Patch file for the molecular viewer, RasMol ver. 2.7.2.1.1.

## Getting Started

This patch enables

-accept GROMACS coordinate file (\*.gro)

-new command "focus on" or "focus number" for controlling viewing point

-output also unitcell with "write vectps" command

## Prerequisites

RasMol_2.7.2.1.1 source

### Installing

patch -p1 < thispatchfile

in the top RasMol_2.7.1.1 source directory.

Then configure & make.

Some 64bit machines require to add

`#define _LONGLONG`

in rasmol.h.

## Authors

Angel M. Bethancourt and Atsushi Masumizu (iCFD: Inst. of Comp. Fluid Dynamics)

Based on the fix at 2018.09.20.
