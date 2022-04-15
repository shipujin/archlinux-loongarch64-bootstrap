### archlinux-loongarch64-bootstrap
Porting distro from scratch is too painful, so arch enthusiasts can focus on their interests and provide a base ARCH environment, which is why the project was set up.


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


