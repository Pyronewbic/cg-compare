# Use case 

```
Custom Cloudera Machine Learning runtimes with Rust so that
we can embed / serve ML models from standalone Rust binaries,
use super-fast ML frameworks s.a. https://github.com/huggingface/candle etc
```

# Short video of CML Rust runtime - multistage building of static Rust binaries orchestrated by K8s/RKE2/Openshift: 

https://youtu.be/w9PLuofxJPI


# Dockerfile from NVIDIA CUDA image

https://github.com/marcredhat/rustcml/blob/main/Dockerfile

```
[root@rhel91 hello_cargo]# docker run --rm --volume /var/run/docker.sock:/var/run/docker.sock --name Grype anchore/grype:latest docker:9fefaea15fd5



NAME                       INSTALLED                   FIXED-IN                    TYPE    VULNERABILITY        SEVERITY
Jinja2                     3.1.2                       3.1.3                       python  GHSA-h5c8-rqwp-cp95  Medium
Pillow                     9.5.0                       10.0.1                      python  GHSA-j7hp-h8jx-5ppr  High
Pillow                     9.5.0                       10.0.0                      python  GHSA-8ghj-p4vj-mr35  High
Pillow                     9.5.0                       10.0.1                      python  GHSA-56pw-mpj4-fxww  High
Pillow                     9.5.0                       10.2.0                      python  GHSA-3f63-hfp8-52jq  High
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48065       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48063       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-47695       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47011       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47010       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47008       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47007       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-45703       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-44840       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2022-35205       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2021-46174       Medium
binutils                   2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2020-19726       Medium
binutils                   2.34-6ubuntu1.6                                         deb     CVE-2019-1010204     Low
binutils                   2.34-6ubuntu1.6                                         deb     CVE-2017-13716       Low
binutils                   2.34-6ubuntu1.6                                         deb     CVE-2022-48064       Negligible
binutils                   2.34-6ubuntu1.6                                         deb     CVE-2018-20657       Negligible
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48065       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48063       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-47695       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47011       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47010       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47008       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47007       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-45703       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-44840       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2022-35205       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2021-46174       Medium
binutils-common            2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2020-19726       Medium
binutils-common            2.34-6ubuntu1.6                                         deb     CVE-2019-1010204     Low
binutils-common            2.34-6ubuntu1.6                                         deb     CVE-2017-13716       Low
binutils-common            2.34-6ubuntu1.6                                         deb     CVE-2022-48064       Negligible
binutils-common            2.34-6ubuntu1.6                                         deb     CVE-2018-20657       Negligible
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48065       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48063       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-47695       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47011       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47010       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47008       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47007       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-45703       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-44840       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2022-35205       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2021-46174       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2020-19726       Medium
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6                                         deb     CVE-2019-1010204     Low
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6                                         deb     CVE-2017-13716       Low
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6                                         deb     CVE-2022-48064       Negligible
binutils-x86-64-linux-gnu  2.34-6ubuntu1.6                                         deb     CVE-2018-20657       Negligible
coreutils                  8.30-3ubuntu2                                           deb     CVE-2016-2781        Low
cpio                       2.13+dfsg-2ubuntu0.3                                    deb     CVE-2023-7207        Medium
cpp                        4:9.3.0-1ubuntu2                                        deb     CVE-2020-13844       Medium
dirmngr                    2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
emacs-bin-common           1:26.3+1-1ubuntu2                                       deb     CVE-2022-48339       Medium
emacs-bin-common           1:26.3+1-1ubuntu2                                       deb     CVE-2022-48337       Medium
emacs-bin-common           1:26.3+1-1ubuntu2                                       deb     CVE-2022-45939       Medium
emacs-common               1:26.3+1-1ubuntu2                                       deb     CVE-2022-48339       Medium
emacs-common               1:26.3+1-1ubuntu2                                       deb     CVE-2022-48337       Medium
emacs-common               1:26.3+1-1ubuntu2                                       deb     CVE-2022-45939       Medium
emacs-nox                  1:26.3+1-1ubuntu2                                       deb     CVE-2022-48339       Medium
emacs-nox                  1:26.3+1-1ubuntu2                                       deb     CVE-2022-48337       Medium
emacs-nox                  1:26.3+1-1ubuntu2                                       deb     CVE-2022-45939       Medium
fonttools                  4.39.3                      4.43.0                      python  GHSA-6673-4983-2vx5  High
g++                        4:9.3.0-1ubuntu2                                        deb     CVE-2020-13844       Medium
gcc                        4:9.3.0-1ubuntu2                                        deb     CVE-2020-13844       Medium
git                        1:2.25.1-1ubuntu3.11                                    deb     CVE-2018-1000021     Low
git-lfs                    2.9.2-1                                                 deb     CVE-2021-21237       Medium
git-man                    1:2.25.1-1ubuntu3.11                                    deb     CVE-2018-1000021     Low
gnupg                      2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gnupg-l10n                 2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gnupg-utils                2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gnupg2                     2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gpg                        2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gpg-agent                  2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gpg-wks-client             2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gpg-wks-server             2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gpgconf                    2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gpgsm                      2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
gpgv                       2.2.19-3ubuntu2.2                                       deb     CVE-2022-3219        Low
jupyter_server             2.5.0                       2.7.2                       python  GHSA-r726-vmfq-j9j3  Medium
jupyter_server             2.5.0                       2.11.2                      python  GHSA-h56g-gq9v-vc8r  Medium
jupyter_server             2.5.0                       2.7.2                       python  GHSA-64x5-55rw-9974  Medium
krb5-multidev              1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
krb5-multidev              1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
krb5-multidev              1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
krb5-user                  1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
krb5-user                  1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
krb5-user                  1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libarchive13               3.4.0-2ubuntu1.2                                        deb     CVE-2022-36227       Low
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48065       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48063       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-47695       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47011       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47010       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47008       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47007       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-45703       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-44840       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2022-35205       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2021-46174       Medium
libbinutils                2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2020-19726       Medium
libbinutils                2.34-6ubuntu1.6                                         deb     CVE-2019-1010204     Low
libbinutils                2.34-6ubuntu1.6                                         deb     CVE-2017-13716       Low
libbinutils                2.34-6ubuntu1.6                                         deb     CVE-2022-48064       Negligible
libbinutils                2.34-6ubuntu1.6                                         deb     CVE-2018-20657       Negligible
libc-bin                   2.31-0ubuntu9.12            2.31-0ubuntu9.14            deb     CVE-2023-4813        Low
libc-bin                   2.31-0ubuntu9.12            2.31-0ubuntu9.14            deb     CVE-2023-4806        Low
libc-bin                   2.31-0ubuntu9.12                                        deb     CVE-2016-20013       Negligible
libc-dev-bin               2.31-0ubuntu9.12            2.31-0ubuntu9.14            deb     CVE-2023-4813        Low
libc-dev-bin               2.31-0ubuntu9.12            2.31-0ubuntu9.14            deb     CVE-2023-4806        Low
libc-dev-bin               2.31-0ubuntu9.12                                        deb     CVE-2016-20013       Negligible
libc6                      2.31-0ubuntu9.12            2.31-0ubuntu9.14            deb     CVE-2023-4813        Low
libc6                      2.31-0ubuntu9.12            2.31-0ubuntu9.14            deb     CVE-2023-4806        Low
libc6                      2.31-0ubuntu9.12                                        deb     CVE-2016-20013       Negligible
libc6-dev                  2.31-0ubuntu9.12            2.31-0ubuntu9.14            deb     CVE-2023-4813        Low
libc6-dev                  2.31-0ubuntu9.12            2.31-0ubuntu9.14            deb     CVE-2023-4806        Low
libc6-dev                  2.31-0ubuntu9.12                                        deb     CVE-2016-20013       Negligible
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48065       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48063       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-47695       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47011       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47010       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47008       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47007       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-45703       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-44840       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2022-35205       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2021-46174       Medium
libctf-nobfd0              2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2020-19726       Medium
libctf-nobfd0              2.34-6ubuntu1.6                                         deb     CVE-2019-1010204     Low
libctf-nobfd0              2.34-6ubuntu1.6                                         deb     CVE-2017-13716       Low
libctf-nobfd0              2.34-6ubuntu1.6                                         deb     CVE-2022-48064       Negligible
libctf-nobfd0              2.34-6ubuntu1.6                                         deb     CVE-2018-20657       Negligible
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48065       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-48063       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.9             deb     CVE-2022-47695       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47011       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47010       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47008       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-47007       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-45703       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.8             deb     CVE-2022-44840       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2022-35205       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2021-46174       Medium
libctf0                    2.34-6ubuntu1.6             2.34-6ubuntu1.7             deb     CVE-2020-19726       Medium
libctf0                    2.34-6ubuntu1.6                                         deb     CVE-2019-1010204     Low
libctf0                    2.34-6ubuntu1.6                                         deb     CVE-2017-13716       Low
libctf0                    2.34-6ubuntu1.6                                         deb     CVE-2022-48064       Negligible
libctf0                    2.34-6ubuntu1.6                                         deb     CVE-2018-20657       Negligible
libdbus-1-3                1.12.16-2ubuntu2.3                                      deb     CVE-2023-34969       Low
libexpat1                  2.2.9-1ubuntu0.6                                        deb     CVE-2023-52426       Medium
libgnutls30                3.6.13-2ubuntu1.8           3.6.13-2ubuntu1.10          deb     CVE-2024-0553        Medium
libgnutls30                3.6.13-2ubuntu1.8           3.6.13-2ubuntu1.9           deb     CVE-2023-5981        Medium
libgssapi-krb5-2           1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
libgssapi-krb5-2           1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
libgssapi-krb5-2           1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libgssrpc4                 1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
libgssrpc4                 1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
libgssrpc4                 1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libk5crypto3               1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
libk5crypto3               1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
libk5crypto3               1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libkadm5clnt-mit11         1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
libkadm5clnt-mit11         1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
libkadm5clnt-mit11         1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libkadm5srv-mit11          1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
libkadm5srv-mit11          1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
libkadm5srv-mit11          1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libkdb5-9                  1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
libkdb5-9                  1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
libkdb5-9                  1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libkrb5-3                  1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
libkrb5-3                  1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
libkrb5-3                  1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libkrb5-dev                1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
libkrb5-dev                1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
libkrb5-dev                1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libkrb5support0            1.17-6ubuntu4.4                                         deb     CVE-2024-26462       Medium
libkrb5support0            1.17-6ubuntu4.4                                         deb     CVE-2024-26461       Medium
libkrb5support0            1.17-6ubuntu4.4                                         deb     CVE-2024-26458       Medium
libldap-2.4-2              2.4.49+dfsg-2ubuntu1.9      2.4.49+dfsg-2ubuntu1.10     deb     CVE-2023-2953        Low
libldap-common             2.4.49+dfsg-2ubuntu1.9      2.4.49+dfsg-2ubuntu1.10     deb     CVE-2023-2953        Low
liblzma-dev                5.2.4-1ubuntu1.1                                        deb     CVE-2020-22916       Medium
liblzma5                   5.2.4-1ubuntu1.1                                        deb     CVE-2020-22916       Medium
libncurses6                6.2-0ubuntu2.1                                          deb     CVE-2023-50495       Low
libncurses6                6.2-0ubuntu2.1                                          deb     CVE-2023-45918       Low
libncursesw5               6.2-0ubuntu2.1                                          deb     CVE-2023-50495       Low
libncursesw5               6.2-0ubuntu2.1                                          deb     CVE-2023-45918       Low
libncursesw6               6.2-0ubuntu2.1                                          deb     CVE-2023-50495       Low
libncursesw6               6.2-0ubuntu2.1                                          deb     CVE-2023-45918       Low
libpam-modules             1.3.1-5ubuntu4.6            1.3.1-5ubuntu4.7            deb     CVE-2024-22365       Medium
libpam-modules-bin         1.3.1-5ubuntu4.6            1.3.1-5ubuntu4.7            deb     CVE-2024-22365       Medium
libpam-runtime             1.3.1-5ubuntu4.6            1.3.1-5ubuntu4.7            deb     CVE-2024-22365       Medium
libpam0g                   1.3.1-5ubuntu4.6            1.3.1-5ubuntu4.7            deb     CVE-2024-22365       Medium
libpcre3                   2:8.39-12ubuntu0.1                                      deb     CVE-2017-11164       Negligible
libperl5.30                5.30.0-9ubuntu0.4           5.30.0-9ubuntu0.5           deb     CVE-2023-47038       Medium
libprocps8                 2:3.3.16-1ubuntu2.3         2:3.3.16-1ubuntu2.4         deb     CVE-2023-4016        Low
libsystemd0                245.4-4ubuntu3.22                                       deb     CVE-2023-7008        Low
libsystemd0                245.4-4ubuntu3.22                                       deb     CVE-2023-26604       Low
libtinfo5                  6.2-0ubuntu2.1                                          deb     CVE-2023-50495       Low
libtinfo5                  6.2-0ubuntu2.1                                          deb     CVE-2023-45918       Low
libtinfo6                  6.2-0ubuntu2.1                                          deb     CVE-2023-50495       Low
libtinfo6                  6.2-0ubuntu2.1                                          deb     CVE-2023-45918       Low
libudev1                   245.4-4ubuntu3.22                                       deb     CVE-2023-7008        Low
libudev1                   245.4-4ubuntu3.22                                       deb     CVE-2023-26604       Low
libzmq3-dev                4.3.2-2ubuntu1                                          deb     CVE-2021-20236       Medium
libzmq3-dev                4.3.2-2ubuntu1                                          deb     CVE-2021-20235       Medium
libzmq3-dev                4.3.2-2ubuntu1                                          deb     CVE-2020-15166       Medium
libzmq5                    4.3.2-2ubuntu1                                          deb     CVE-2021-20236       Medium
libzmq5                    4.3.2-2ubuntu1                                          deb     CVE-2021-20235       Medium
libzmq5                    4.3.2-2ubuntu1                                          deb     CVE-2020-15166       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-1086        High
linux-libc-dev             5.4.0-166.183               5.4.0-172.190               deb     CVE-2024-0646        High
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-0584        High
linux-libc-dev             5.4.0-166.183               5.4.0-170.188               deb     CVE-2023-6932        High
linux-libc-dev             5.4.0-166.183               5.4.0-170.188               deb     CVE-2023-6931        High
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-6176        High
linux-libc-dev             5.4.0-166.183               5.4.0-172.190               deb     CVE-2023-51781       High
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-4563        High
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-4244        High
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-20569       High
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-24855       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-23307       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-0841        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-0775        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-0639        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-0607        Medium
linux-libc-dev             5.4.0-166.183               5.4.0-172.190               deb     CVE-2024-0565        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-0564        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-7042        Medium
linux-libc-dev             5.4.0-166.183               5.4.0-172.190               deb     CVE-2023-6915        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-6610        Medium
linux-libc-dev             5.4.0-166.183               5.4.0-170.188               deb     CVE-2023-6606        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-6121        Medium
linux-libc-dev             5.4.0-166.183               5.4.0-170.188               deb     CVE-2023-6040        Medium
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-5717        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-51782       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-51780       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-5178        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-51779       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-51043       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-51042       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-46838       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-171.189               deb     CVE-2023-46343       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-167.184               deb     CVE-2023-45871       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-171.189               deb     CVE-2023-45863       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-42754       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-39198       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-39194       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-39193       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-39192       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-39189       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-37453       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-171.189               deb     CVE-2023-34324       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-31082       Medium
linux-libc-dev             5.4.0-166.183               5.4.0-169.187               deb     CVE-2023-3006        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-28327       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-26242       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-23004       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-23000       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-2007        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-1582        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-0160        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-0030        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-48619       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-4543        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-40133       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-39189       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-38457       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-38096       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-36402       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-3523        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-3344        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-29900       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-2961        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-25836       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-1280        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-1247        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-0480        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-0400        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2021-4148        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2021-3864        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-36766       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-36310       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-27835       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-26144       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-24504       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-12362       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2018-17977       Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2016-8660        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2015-8553        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2013-7445        Medium
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-23851       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-23849       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2024-0340        Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-47233       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-4134        Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-4133        Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-4010        Low
linux-libc-dev             5.4.0-166.183               5.4.0-171.189               deb     CVE-2023-35827       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-33288       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-33053       Low
linux-libc-dev             5.4.0-166.183               5.4.0-167.184               deb     CVE-2023-31085       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-22995       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2023-1989        Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-47519       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-47518       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-45885       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-45884       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-0854        Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2021-44879       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2021-34981       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2021-33631       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-35501       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-14304       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-12364       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2020-12363       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2019-19814       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2019-19378       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2019-15213       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2019-14899       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2018-12931       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2018-12930       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2018-12929       Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2018-1121        Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2017-0537        Low
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-44034       Negligible
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-44033       Negligible
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-44032       Negligible
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2022-41848       Negligible
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2021-39801       Negligible
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2021-32078       Negligible
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2021-26934       Negligible
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2018-12928       Negligible
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2017-13693       Negligible
linux-libc-dev             5.4.0-166.183                                           deb     CVE-2017-13165       Negligible
locales                    2.31-0ubuntu9.14                                        deb     CVE-2016-20013       Negligible
login                      1:4.8.1-1ubuntu5.20.04.4    1:4.8.1-1ubuntu5.20.04.5    deb     CVE-2023-4641        Low
login                      1:4.8.1-1ubuntu5.20.04.4                                deb     CVE-2023-29383       Low
login                      1:4.8.1-1ubuntu5.20.04.4                                deb     CVE-2013-4235        Low
ncurses-base               6.2-0ubuntu2.1                                          deb     CVE-2023-50495       Low
ncurses-base               6.2-0ubuntu2.1                                          deb     CVE-2023-45918       Low
ncurses-bin                6.2-0ubuntu2.1                                          deb     CVE-2023-50495       Low
ncurses-bin                6.2-0ubuntu2.1                                          deb     CVE-2023-45918       Low
openssh-client             1:8.2p1-4ubuntu0.11                                     deb     CVE-2023-51767       Medium
openssh-server             1:8.2p1-4ubuntu0.11                                     deb     CVE-2023-51767       Medium
openssh-sftp-server        1:8.2p1-4ubuntu0.11                                     deb     CVE-2023-51767       Medium
openssl                    1.1.1f-1ubuntu2.20          1.1.1f-1ubuntu2.21          deb     CVE-2024-0727        Low
openssl                    1.1.1f-1ubuntu2.20          1.1.1f-1ubuntu2.21          deb     CVE-2023-5678        Low
passwd                     1:4.8.1-1ubuntu5.20.04.4    1:4.8.1-1ubuntu5.20.04.5    deb     CVE-2023-4641        Low
passwd                     1:4.8.1-1ubuntu5.20.04.4                                deb     CVE-2023-29383       Low
passwd                     1:4.8.1-1ubuntu5.20.04.4                                deb     CVE-2013-4235        Low
patch                      2.7.6-6                                                 deb     CVE-2021-45261       Negligible
patch                      2.7.6-6                                                 deb     CVE-2018-6952        Negligible
perl                       5.30.0-9ubuntu0.4           5.30.0-9ubuntu0.5           deb     CVE-2023-47038       Medium
perl-base                  5.30.0-9ubuntu0.4           5.30.0-9ubuntu0.5           deb     CVE-2023-47038       Medium
perl-modules-5.30          5.30.0-9ubuntu0.4           5.30.0-9ubuntu0.5           deb     CVE-2023-47038       Medium
pip                        23.1.2                      23.3                        python  GHSA-mq26-g339-26xf  Medium
procps                     2:3.3.16-1ubuntu2.3         2:3.3.16-1ubuntu2.4         deb     CVE-2023-4016        Low
python                     3.10.9                                                  binary  CVE-2023-36632       High
python                     3.10.9                                                  binary  CVE-2023-24329       High
python                     3.10.9                                                  binary  CVE-2023-40217       Medium
python                     3.10.9                                                  binary  CVE-2023-27043       Medium
python                     3.10.9                                                  binary  CVE-2007-4559        Medium
setuptools                 65.5.0                      65.5.1                      python  GHSA-r9hx-vwmv-q579  High
ssh                        1:8.2p1-4ubuntu0.11                                     deb     CVE-2023-51767       Medium
tar                        1.30+dfsg-7ubuntu0.20.04.3  1.30+dfsg-7ubuntu0.20.04.4  deb     CVE-2023-39804       Medium
tornado                    6.3.2                       6.3.3                       python  GHSA-qppv-j76h-2rpx  Medium
urllib3                    1.26.15                     1.26.17                     python  GHSA-v845-jxx5-vc9f  Medium
urllib3                    1.26.15                     1.26.18                     python  GHSA-g4mx-q9vg-27p4  Medium
wget                       1.20.3-1ubuntu2                                         deb     CVE-2021-31879       Medium
xz-utils                   5.2.4-1ubuntu1.1                                        deb     CVE-2020-22916       Medium
```

# Dockerfile from ChainGuard pytorch CUDA image

https://github.com/marcredhat/rustcml/blob/main/Dockerfile.cuda.chainguard

```
[root@rhel91 chainguard]# docker run --rm --volume /var/run/docker.sock:/var/run/docker.sock --name Grype anchore/grype:latest docker:bb3c4ff5e4e7 > grypechain

[root@rhel91 chainguard]# cat grypechain
NAME        INSTALLED  FIXED-IN  TYPE    VULNERABILITY        SEVERITY
pip         23.1.2     23.3      python  GHSA-mq26-g339-26xf  Medium
python      3.10.9               binary  CVE-2023-36632       High
python      3.10.9               binary  CVE-2023-24329       High
python      3.10.9               binary  CVE-2023-40217       Medium
python      3.10.9               binary  CVE-2023-27043       Medium
python      3.10.9               binary  CVE-2007-4559        Medium
setuptools  65.5.0     65.5.1    python  GHSA-r9hx-vwmv-q579  High
```


