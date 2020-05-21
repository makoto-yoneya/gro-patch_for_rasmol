# rasmol-gro

Patch file for [RasMol][1] ver. 2.7.2.1.1.

## Functions

This patch enables

- accept GROMACS coordinate file (\*.gro)

- new command "focus on" or "focus number" for controlling viewing point

- output also unitcell with "write vectps" command

## Prerequisites

RasMol_2.7.2.1.1 source: [RasMol_2.7.2.1.1.tar.gz][2]

### Installing

`patch -p1 < RasMol_2.7.2.1.1-gro.patch`

in the top source directory and make.

Some 64bit machines require to add

`#define _LONGLONG`

in rasmol.h.

## Authors

Angel M. Bethancourt and Atsushi Masumizu (iCFD: Inst. of Comp. Fluid Dynamics)

Based on the fix at 2018.09.20.

[1]: http://www.openrasmol.org/
[2]: http://www.bernstein-plus-sons.com/software/RasMol_2.7.2.1.1.tar.gz
