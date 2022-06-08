### archlinux-loongarch64-bootstrap
Porting distro from scratch is too painful, so arch enthusiasts can focus on their interests and provide a base ARCH environment, which is why the project was set up.


#### tag:0.4 archlinux-bootstrap-2022.05.25-loongarch64
1. Archlinux Loongarch64 toolchain gcc/glibc/binutils

```
# Set up archLinux loongarch64 repository and build archlinux-bootstrap-2022.05.25-loongarch64-rootfs using Pacstrap
# virtual address repository (virtual address: http://pkg.iloongarch.cn/archlinux/repo/virtual-address
pacstrap `pwd`/mnt base-devel gcc glibc binutils linux

chroot `pwd`/mnt
pacman -Q gcc glibc binutils linux
gcc 12.1.0-7
glibc 2.36-6
binutils 2.38.50-5
linux 5.17.0_rc1-2
```
2. Archlinux loongarch64 xfce4 graphics desktop (physical Address vault is in progress):

```
Web site home: http://pkg.iloongarch.cn/archlinux
BBS: https://bbs.loongarch.org/d/31-loongarch-archlinux-bootstrap
virtual address repository(virtual address: http://pkg.iloongarch.cn/archlinux/repo/virtual-address
physical address repository(physical address, the repository is under way) : http://pkg.iloongarch.cn/archlinux/repo
```

3. Archlinux Loongarch64 PKGBUILD

```
core: https://github.com/archlinux-loongarch64/core
extra: https://github.com/archlinux-loongarch64/extra
community: https://github.com/archlinux-loongarch64/community
```

| package | branch | commit hash | url |
| ---- | ---- | ---- | ---- |
| binutils | 2.38 release | 9c67f6382ac2c90fbde5729feaf7d59ce662147a | https://sourceware.org/git/binutils-gdb.git |
| gcc | 12.1.0 release | release | https://ftp.gnu.org/gnu/gcc/gcc-12.1.0/gcc-12.1.0.tar.xz |
| glibc | loongarch_2_36_dev_v4 | 29a3ed2ec825b72d0def7cb51b3998615abf8c6b | https://github.com/loongson/glibc.git |
| linux | loongarch-next | 3643df5f058aacf69ac4121f6882500e843b7a34 | https://github.com/loongson/linux.git |
| systemd | dev-loongarch | 6d39da79c85d35e95d3993fa6b8873fccda33bd9 | https://github.com/loongarch64/systemd.git |
| libffi | loongarch-3_4_2 | 70602040e7a319ad4131aad422d59a493bc65f18 | https://github.com/loongson/libffi.git |
| libseccomp | dev-main | 5b4ba10fd1a9ad5baa85ebecafd36c401a030788 |https://github.com/loongarch64/libseccomp.git |


#### tag:0.3 archlinux-bootstrap-2022.04.15-loongarch64

1. Upgrade using the latest basic software version (github.com/loongson: gcc/binutils/glibc)
2. Add basic tools: meson, ninja, cmake
3. Add the preinstalled software list file pkglist.loongarch64.txt

| package | branch | commit hash | url |
| ---- | ---- | ---- | ---- |
| binutils | upstream_v4.1 | f9b0887de1111349310acf79326f6b33bb0cc221 | https://github.com/loongson/binutils-gdb.git |
| gcc | loongarch-12 | e7d20cc74d581de32effac595a673f27b7fec826 | https://github.com/loongson/gcc.git |
| glibc | loongarch_2_36_dev_v3 | 24471ad8e7f0e7523809bf789b47f910b3a47315 | https://github.com/loongson/glibc.git |
| linux | loongarch-next | 3643df5f058aacf69ac4121f6882500e843b7a34 | https://github.com/loongson/linux.git |
| systemd | dev-loongarch | 350489abb1c9ce4e43dab54b7af7d1a1bfbfb3b8 | https://github.com/loongarch64/systemd.git |
| libffi | loongarch-3_4_2 | 70602040e7a319ad4131aad422d59a493bc65f18 | https://github.com/loongson/libffi.git |
| libseccomp | dev-main | 5b4ba10fd1a9ad5baa85ebecafd36c401a030788 |https://github.com/loongarch64/libseccomp.git |

#### tag:0.2 archlinux-bootstrap-2022.03.18-loongarch64

* Fixed some software path issues

| package | branch | commit hash | url |
| ---- | ---- | ---- | ---- |
| binutils | upstream_v3.1 | f51838f4b4e0153acdf4a9849c17675775577cda | https://github.com/loongson/binutils-gdb.git |
| gcc | loongarch_upstream_v6.3 | 78c693aa2d833bfa27907141ba8bf93123b45567 | https://github.com/loongson/gcc.git |
| glibc | loongarch_2_35_dev_v2.2 | 74492b6d4613976aff5a9091a93d6ed4407d70a9 | https://github.com/loongson/glibc.git |
| linux | loongarch-next | 3643df5f058aacf69ac4121f6882500e843b7a34 | https://github.com/loongson/linux.git |
| systemd | dev-loongarch | 350489abb1c9ce4e43dab54b7af7d1a1bfbfb3b8 | https://github.com/loongarch64/systemd.git |
| libffi | loongarch-3_4_2 | 70602040e7a319ad4131aad422d59a493bc65f18 | https://github.com/loongson/libffi.git |
| libseccomp | dev-main | 5b4ba10fd1a9ad5baa85ebecafd36c401a030788 |https://github.com/loongarch64/libseccomp.git |

#### tag:0.1 archlinux-bootstrap-2022.03.17-loongarch64
| package | version | url |
| ---- | ---- | ---- |
| binutils | upstream_v3.1 | https://github.com/loongson/binutils-gdb.git |
| gcc | loongarch_upstream_v6.3 | https://github.com/loongson/gcc.git |
| glibc | loongarch_2_35_dev_v2.2 | https://github.com/loongson/glibc.git |
| linux | loongarch-next | https://github.com/loongson/linux.git |
| systemd | dev-loongarch | https://github.com/loongarch64/systemd.git |
| libffi | loongarch-3_4_2 | https://github.com/loongson/libffi.git |
| libseccomp | dev-main | https://github.com/loongarch64/libseccomp.git |


