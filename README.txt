riscv64--glibc--bleeding-edge-2018.11-1


Toolchains are hosted here: http://toolchains.bootlin.com/

All the licenses can be found here: http://toolchains.bootlin.com/downloads/releases/licenses/
All the sources can be found here: http://toolchains.bootlin.com/downloads/releases/sources/

PACKAGE      VERSION                     LICENSE
buildroot    2018.11-rc2-00003-ga0787e9  GPL-2.0+
gcc-final    8.2.0                       unknown
bison        3.0.4                       GPL-3.0+
lzip         1.20                        GPL-2.0+
m4           1.4.18                      GPL-3.0+
gawk         4.2.1                       GPL-3.0+
gcc-initial  8.2.0                       unknown
binutils     2.31.1                      GPL-3.0+, libiberty LGPL-2.1+
gmp          6.1.2                       LGPL-3.0+ or GPL-2.0+
mpc          1.0.3                       LGPL-3.0+
mpfr         3.1.6                       LGPL-3.0+
patchelf     0.9                         GPL-3.0+
glibc          glibc-2.28-18-g2339d6a55eb7a7e040ae888e906adc49eeb59eab  GPL-2.0+ (programs), LGPL-2.1+, BSD-3-Clause, MIT (library)
linux-headers  4.18.18                                                  GPL-2.0
dash           0.5.10.2                                                 BSD-3-Clause, GPL-2.0+ (mksignames.c)

For those who would like to reproduce the toolchain, you can just follow these steps:

    git clone https://github.com/bootlin/buildroot-toolchains.git buildroot
    cd buildroot
    git checkout toolchains.bootlin.com-bleeding-edge-2018.11-1

    curl http://toolchains.bootlin.com/downloads/releases/toolchains/riscv64/build_fragments/riscv64--glibc--bleeding-edge-2018.11-1.defconfig > .config
    make olddefconfig
    make

This toolchain has been built, but the infrastructure does not contains enough
informations about testing it.
This doesn't mean that this toolchain doesn't work, just that it hasn't been
fully tested.
FLAG: CAN-NOT-TEST
