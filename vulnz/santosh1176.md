## Golang-server

```shell
a0557@cve-bliss:santoshdts$ grype santoshdts/server:go
 ✔ Vulnerability DB                [no update available]  
 ✔ Loaded image                                                                                                                                                                                       santoshdts/server:go
 ✔ Parsed image                                                                                                                                    sha256:f0b736f8fb0a14652645df7b1a181790b4f25d8615ed70a884ff59c19c37a3aa
 ✔ Cataloged contents                                                                                                                                     f86a5fb1972dde8ff8a7e87c51cc578efc09490cd56cec2bc83a785a2be422de
   ├── ✔ Packages                        [249 packages]  
   ├── ✔ File digests                    [12,901 files]  
   ├── ✔ File metadata                   [12,901 locations]  
   └── ✔ Executables                     [1,069 executables]  
 ✔ Scanned for vulnerabilities     [358 vulnerability matches]  
   ├── by severity: 1 critical, 34 high, 81 medium, 8 low, 228 negligible (6 unknown)
   └── by status:   0 fixed, 358 not-fixed, 0 ignored 
[0009]  WARN cataloger failed cataloger=java-archive-cataloger error=unable to read files from java archive: unable to open zip archive (/tmp/syft-archive-contents-619634932/archive-test-badbase.zip): unable to open ZipR
[0009]  WARN cataloger failed cataloger=java-archive-cataloger error=unable to read files from java archive: unable to open zip archive (/tmp/syft-archive-contents-1997391525/archive-test-baddirsz.zip): unable to open Zi
[0010]  WARN cataloger failed cataloger=linux-kernel-cataloger error=unable to get magic type for file: EOF location=/usr/local/go/src/debug/pe/testdata/vmlinuz-4.15.0-47-generic
[0011]  WARN unable to process executable "/usr/local/go/src/debug/pe/testdata/vmlinuz-4.15.0-47-generic" error=unable to determine executable kind: unable to read enough bytes to determine executable format
NAME                       INSTALLED              FIXED-IN     TYPE  VULNERABILITY     SEVERITY   
apt                        2.6.1                               deb   CVE-2011-3374     Negligible  
binutils                   2.40-2                              deb   CVE-2023-1972     Negligible  
binutils                   2.40-2                              deb   CVE-2021-32256    Negligible  
binutils                   2.40-2                              deb   CVE-2018-9996     Negligible  
binutils                   2.40-2                              deb   CVE-2018-20712    Negligible  
binutils                   2.40-2                              deb   CVE-2018-20673    Negligible  
binutils                   2.40-2                              deb   CVE-2018-18483    Negligible  
binutils                   2.40-2                              deb   CVE-2017-13716    Negligible  
binutils-common            2.40-2                              deb   CVE-2023-1972     Negligible  
binutils-common            2.40-2                              deb   CVE-2021-32256    Negligible  
binutils-common            2.40-2                              deb   CVE-2018-9996     Negligible  
binutils-common            2.40-2                              deb   CVE-2018-20712    Negligible  
binutils-common            2.40-2                              deb   CVE-2018-20673    Negligible  
binutils-common            2.40-2                              deb   CVE-2018-18483    Negligible  
binutils-common            2.40-2                              deb   CVE-2017-13716    Negligible  
binutils-x86-64-linux-gnu  2.40-2                              deb   CVE-2023-1972     Negligible  
binutils-x86-64-linux-gnu  2.40-2                              deb   CVE-2021-32256    Negligible  
binutils-x86-64-linux-gnu  2.40-2                              deb   CVE-2018-9996     Negligible  
binutils-x86-64-linux-gnu  2.40-2                              deb   CVE-2018-20712    Negligible  
binutils-x86-64-linux-gnu  2.40-2                              deb   CVE-2018-20673    Negligible  
binutils-x86-64-linux-gnu  2.40-2                              deb   CVE-2018-18483    Negligible  
binutils-x86-64-linux-gnu  2.40-2                              deb   CVE-2017-13716    Negligible  
bsdutils                   1:2.38.1-5+b1                       deb   CVE-2022-0563     Negligible  
coreutils                  9.1-1                  (won't fix)  deb   CVE-2016-2781     Low         
coreutils                  9.1-1                               deb   CVE-2017-18018    Negligible  
cpp-12                     12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
cpp-12                     12.2.0-14                           deb   CVE-2022-27943    Negligible  
dirmngr                    2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
g++-12                     12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
g++-12                     12.2.0-14                           deb   CVE-2022-27943    Negligible  
gcc-12                     12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
gcc-12                     12.2.0-14                           deb   CVE-2022-27943    Negligible  
gcc-12-base                12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
gcc-12-base                12.2.0-14                           deb   CVE-2022-27943    Negligible  
git                        1:2.39.2-1.1           (won't fix)  deb   CVE-2023-29007    High        
git                        1:2.39.2-1.1           (won't fix)  deb   CVE-2023-25652    High        
git                        1:2.39.2-1.1           (won't fix)  deb   CVE-2023-25815    Low         
git                        1:2.39.2-1.1                        deb   CVE-2022-24975    Negligible  
git                        1:2.39.2-1.1                        deb   CVE-2018-1000021  Negligible  
git-man                    1:2.39.2-1.1           (won't fix)  deb   CVE-2023-29007    High        
git-man                    1:2.39.2-1.1           (won't fix)  deb   CVE-2023-25652    High        
git-man                    1:2.39.2-1.1           (won't fix)  deb   CVE-2023-25815    Low         
git-man                    1:2.39.2-1.1                        deb   CVE-2022-24975    Negligible  
git-man                    1:2.39.2-1.1                        deb   CVE-2018-1000021  Negligible  
gnupg                      2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
gnupg-l10n                 2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
gnupg-utils                2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
gpg                        2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
gpg-agent                  2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
gpg-wks-client             2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
gpg-wks-server             2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
gpgconf                    2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
gpgsm                      2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
gpgv                       2.2.40-1.1                          deb   CVE-2022-3219     Negligible  
libapt-pkg6.0              2.6.1                               deb   CVE-2011-3374     Negligible  
libasan8                   12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libasan8                   12.2.0-14                           deb   CVE-2022-27943    Negligible  
libatomic1                 12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libatomic1                 12.2.0-14                           deb   CVE-2022-27943    Negligible  
libbinutils                2.40-2                              deb   CVE-2023-1972     Negligible  
libbinutils                2.40-2                              deb   CVE-2021-32256    Negligible  
libbinutils                2.40-2                              deb   CVE-2018-9996     Negligible  
libbinutils                2.40-2                              deb   CVE-2018-20712    Negligible  
libbinutils                2.40-2                              deb   CVE-2018-20673    Negligible  
libbinutils                2.40-2                              deb   CVE-2018-18483    Negligible  
libbinutils                2.40-2                              deb   CVE-2017-13716    Negligible  
libblkid1                  2.38.1-5+b1                         deb   CVE-2022-0563     Negligible  
libc-bin                   2.36-9+deb12u4                      deb   CVE-2019-9192     Negligible  
libc-bin                   2.36-9+deb12u4                      deb   CVE-2019-1010025  Negligible  
libc-bin                   2.36-9+deb12u4                      deb   CVE-2019-1010024  Negligible  
libc-bin                   2.36-9+deb12u4                      deb   CVE-2019-1010023  Negligible  
libc-bin                   2.36-9+deb12u4                      deb   CVE-2019-1010022  Negligible  
libc-bin                   2.36-9+deb12u4                      deb   CVE-2018-20796    Negligible  
libc-bin                   2.36-9+deb12u4                      deb   CVE-2010-4756     Negligible  
libc-dev-bin               2.36-9+deb12u4                      deb   CVE-2019-9192     Negligible  
libc-dev-bin               2.36-9+deb12u4                      deb   CVE-2019-1010025  Negligible  
libc-dev-bin               2.36-9+deb12u4                      deb   CVE-2019-1010024  Negligible  
libc-dev-bin               2.36-9+deb12u4                      deb   CVE-2019-1010023  Negligible  
libc-dev-bin               2.36-9+deb12u4                      deb   CVE-2019-1010022  Negligible  
libc-dev-bin               2.36-9+deb12u4                      deb   CVE-2018-20796    Negligible  
libc-dev-bin               2.36-9+deb12u4                      deb   CVE-2010-4756     Negligible  
libc6                      2.36-9+deb12u4                      deb   CVE-2019-9192     Negligible  
libc6                      2.36-9+deb12u4                      deb   CVE-2019-1010025  Negligible  
libc6                      2.36-9+deb12u4                      deb   CVE-2019-1010024  Negligible  
libc6                      2.36-9+deb12u4                      deb   CVE-2019-1010023  Negligible  
libc6                      2.36-9+deb12u4                      deb   CVE-2019-1010022  Negligible  
libc6                      2.36-9+deb12u4                      deb   CVE-2018-20796    Negligible  
libc6                      2.36-9+deb12u4                      deb   CVE-2010-4756     Negligible  
libc6-dev                  2.36-9+deb12u4                      deb   CVE-2019-9192     Negligible  
libc6-dev                  2.36-9+deb12u4                      deb   CVE-2019-1010025  Negligible  
libc6-dev                  2.36-9+deb12u4                      deb   CVE-2019-1010024  Negligible  
libc6-dev                  2.36-9+deb12u4                      deb   CVE-2019-1010023  Negligible  
libc6-dev                  2.36-9+deb12u4                      deb   CVE-2019-1010022  Negligible  
libc6-dev                  2.36-9+deb12u4                      deb   CVE-2018-20796    Negligible  
libc6-dev                  2.36-9+deb12u4                      deb   CVE-2010-4756     Negligible  
libcc1-0                   12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libcc1-0                   12.2.0-14                           deb   CVE-2022-27943    Negligible  
libctf-nobfd0              2.40-2                              deb   CVE-2023-1972     Negligible  
libctf-nobfd0              2.40-2                              deb   CVE-2021-32256    Negligible  
libctf-nobfd0              2.40-2                              deb   CVE-2018-9996     Negligible  
libctf-nobfd0              2.40-2                              deb   CVE-2018-20712    Negligible  
libctf-nobfd0              2.40-2                              deb   CVE-2018-20673    Negligible  
libctf-nobfd0              2.40-2                              deb   CVE-2018-18483    Negligible  
libctf-nobfd0              2.40-2                              deb   CVE-2017-13716    Negligible  
libctf0                    2.40-2                              deb   CVE-2023-1972     Negligible  
libctf0                    2.40-2                              deb   CVE-2021-32256    Negligible  
libctf0                    2.40-2                              deb   CVE-2018-9996     Negligible  
libctf0                    2.40-2                              deb   CVE-2018-20712    Negligible  
libctf0                    2.40-2                              deb   CVE-2018-20673    Negligible  
libctf0                    2.40-2                              deb   CVE-2018-18483    Negligible  
libctf0                    2.40-2                              deb   CVE-2017-13716    Negligible  
libexpat1                  2.5.0-1                             deb   CVE-2023-52425    High        
libexpat1                  2.5.0-1                             deb   CVE-2023-52426    Medium      
libgcc-12-dev              12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libgcc-12-dev              12.2.0-14                           deb   CVE-2022-27943    Negligible  
libgcc-s1                  12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libgcc-s1                  12.2.0-14                           deb   CVE-2022-27943    Negligible  
libgcrypt20                1.10.1-3                            deb   CVE-2018-6829     Negligible  
libgnutls30                3.7.9-2+deb12u2                     deb   CVE-2011-3389     Negligible  
libgomp1                   12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libgomp1                   12.2.0-14                           deb   CVE-2022-27943    Negligible  
libgprofng0                2.40-2                              deb   CVE-2023-1972     Negligible  
libgprofng0                2.40-2                              deb   CVE-2021-32256    Negligible  
libgprofng0                2.40-2                              deb   CVE-2018-9996     Negligible  
libgprofng0                2.40-2                              deb   CVE-2018-20712    Negligible  
libgprofng0                2.40-2                              deb   CVE-2018-20673    Negligible  
libgprofng0                2.40-2                              deb   CVE-2018-18483    Negligible  
libgprofng0                2.40-2                              deb   CVE-2017-13716    Negligible  
libgssapi-krb5-2           1.20.1-2+deb12u1                    deb   CVE-2018-5709     Negligible  
libitm1                    12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libitm1                    12.2.0-14                           deb   CVE-2022-27943    Negligible  
libjansson4                2.14-2                              deb   CVE-2020-36325    Negligible  
libk5crypto3               1.20.1-2+deb12u1                    deb   CVE-2018-5709     Negligible  
libkrb5-3                  1.20.1-2+deb12u1                    deb   CVE-2018-5709     Negligible  
libkrb5support0            1.20.1-2+deb12u1                    deb   CVE-2018-5709     Negligible  
libldap-2.5-0              2.5.13+dfsg-5          (won't fix)  deb   CVE-2023-2953     High        
libldap-2.5-0              2.5.13+dfsg-5                       deb   CVE-2020-15719    Negligible  
libldap-2.5-0              2.5.13+dfsg-5                       deb   CVE-2017-17740    Negligible  
libldap-2.5-0              2.5.13+dfsg-5                       deb   CVE-2017-14159    Negligible  
libldap-2.5-0              2.5.13+dfsg-5                       deb   CVE-2015-3276     Negligible  
liblsan0                   12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
liblsan0                   12.2.0-14                           deb   CVE-2022-27943    Negligible  
libmount1                  2.38.1-5+b1                         deb   CVE-2022-0563     Negligible  
libncursesw6               6.4-4                  (won't fix)  deb   CVE-2023-50495    Medium      
libpam-modules             1.5.2-6+deb12u1        (won't fix)  deb   CVE-2024-22365    Medium      
libpam-modules-bin         1.5.2-6+deb12u1        (won't fix)  deb   CVE-2024-22365    Medium      
libpam-runtime             1.5.2-6+deb12u1        (won't fix)  deb   CVE-2024-22365    Medium      
libpam0g                   1.5.2-6+deb12u1        (won't fix)  deb   CVE-2024-22365    Medium      
libperl5.36                5.36.0-7+deb12u1       (won't fix)  deb   CVE-2023-31484    High        
libperl5.36                5.36.0-7+deb12u1                    deb   CVE-2023-31486    Negligible  
libperl5.36                5.36.0-7+deb12u1                    deb   CVE-2011-4116     Negligible  
libproc2-0                 2:4.0.2-3              (won't fix)  deb   CVE-2023-4016     Low         
libpython3.11-minimal      3.11.2-6               (won't fix)  deb   CVE-2023-41105    High        
libpython3.11-minimal      3.11.2-6               (won't fix)  deb   CVE-2023-24329    High        
libpython3.11-minimal      3.11.2-6               (won't fix)  deb   CVE-2023-40217    Medium      
libpython3.11-minimal      3.11.2-6               (won't fix)  deb   CVE-2023-27043    Medium      
libpython3.11-minimal      3.11.2-6                            deb   CVE-2023-24535    Negligible  
libpython3.11-stdlib       3.11.2-6               (won't fix)  deb   CVE-2023-41105    High        
libpython3.11-stdlib       3.11.2-6               (won't fix)  deb   CVE-2023-24329    High        
libpython3.11-stdlib       3.11.2-6               (won't fix)  deb   CVE-2023-40217    Medium      
libpython3.11-stdlib       3.11.2-6               (won't fix)  deb   CVE-2023-27043    Medium      
libpython3.11-stdlib       3.11.2-6                            deb   CVE-2023-24535    Negligible  
libquadmath0               12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libquadmath0               12.2.0-14                           deb   CVE-2022-27943    Negligible  
libsmartcols1              2.38.1-5+b1                         deb   CVE-2022-0563     Negligible  
libsqlite3-0               3.40.1-2               (won't fix)  deb   CVE-2023-7104     High        
libsqlite3-0               3.40.1-2               (won't fix)  deb   CVE-2024-0232     Medium      
libsqlite3-0               3.40.1-2                            deb   CVE-2021-45346    Negligible  
libssl3                    3.0.11-1~deb12u2       (won't fix)  deb   CVE-2024-0727     Medium      
libssl3                    3.0.11-1~deb12u2       (won't fix)  deb   CVE-2023-6129     Medium      
libssl3                    3.0.11-1~deb12u2       (won't fix)  deb   CVE-2023-5678     Medium      
libssl3                    3.0.11-1~deb12u2                    deb   CVE-2010-0928     Negligible  
libssl3                    3.0.11-1~deb12u2                    deb   CVE-2007-6755     Negligible  
libssl3                    3.0.11-1~deb12u2       (won't fix)  deb   CVE-2023-6237     Unknown     
libstdc++-12-dev           12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libstdc++-12-dev           12.2.0-14                           deb   CVE-2022-27943    Negligible  
libstdc++6                 12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libstdc++6                 12.2.0-14                           deb   CVE-2022-27943    Negligible  
libsystemd0                252.22-1~deb12u1                    deb   CVE-2023-31439    Negligible  
libsystemd0                252.22-1~deb12u1                    deb   CVE-2023-31438    Negligible  
libsystemd0                252.22-1~deb12u1                    deb   CVE-2023-31437    Negligible  
libsystemd0                252.22-1~deb12u1                    deb   CVE-2013-4392     Negligible  
libtinfo6                  6.4-4                  (won't fix)  deb   CVE-2023-50495    Medium      
libtsan2                   12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libtsan2                   12.2.0-14                           deb   CVE-2022-27943    Negligible  
libubsan1                  12.2.0-14              (won't fix)  deb   CVE-2023-4039     Medium      
libubsan1                  12.2.0-14                           deb   CVE-2022-27943    Negligible  
libudev1                   252.22-1~deb12u1                    deb   CVE-2023-31439    Negligible  
libudev1                   252.22-1~deb12u1                    deb   CVE-2023-31438    Negligible  
libudev1                   252.22-1~deb12u1                    deb   CVE-2023-31437    Negligible  
libudev1                   252.22-1~deb12u1                    deb   CVE-2013-4392     Negligible  
libuuid1                   2.38.1-5+b1                         deb   CVE-2022-0563     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2024-23307    High        
linux-libc-dev             6.1.76-1                            deb   CVE-2024-21803    High        
linux-libc-dev             6.1.76-1                            deb   CVE-2024-0841     High        
linux-libc-dev             6.1.76-1                            deb   CVE-2023-6536     High        
linux-libc-dev             6.1.76-1                            deb   CVE-2023-6535     High        
linux-libc-dev             6.1.76-1                            deb   CVE-2023-6356     High        
linux-libc-dev             6.1.76-1                            deb   CVE-2023-6270     High        
linux-libc-dev             6.1.76-1                            deb   CVE-2023-3640     High        
linux-libc-dev             6.1.76-1                            deb   CVE-2023-2176     High        
linux-libc-dev             6.1.76-1                            deb   CVE-2021-3864     High        
linux-libc-dev             6.1.76-1                            deb   CVE-2021-3847     High        
linux-libc-dev             6.1.76-1               (won't fix)  deb   CVE-2019-19814    High        
linux-libc-dev             6.1.76-1               (won't fix)  deb   CVE-2019-19449    High        
linux-libc-dev             6.1.76-1               (won't fix)  deb   CVE-2013-7445     High        
linux-libc-dev             6.1.76-1                            deb   CVE-2024-24864    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-24861    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-24860    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-24859    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-24858    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-24857    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-24855    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-23851    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-23850    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-23848    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-23196    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-22386    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-22099    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-1151     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-0564     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2024-0340     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-7042     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-6240     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-6039     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-47233    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-4133     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-4010     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-37454    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-3397     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-31083    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-31082    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-23005    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-21264    Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-1192     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-0597     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2023-0160     Medium      
linux-libc-dev             6.1.76-1               (won't fix)  deb   CVE-2022-4543     Medium      
linux-libc-dev             6.1.76-1                            deb   CVE-2020-36694    Medium      
linux-libc-dev             6.1.76-1               (won't fix)  deb   CVE-2020-14304    Medium      
linux-libc-dev             6.1.76-1               (won't fix)  deb   CVE-2019-20794    Medium      
linux-libc-dev             6.1.76-1               (won't fix)  deb   CVE-2019-16089    Medium      
linux-libc-dev             6.1.76-1               (won't fix)  deb   CVE-2019-15213    Medium      
linux-libc-dev             6.1.76-1               (won't fix)  deb   CVE-2018-12928    Low         
linux-libc-dev             6.1.76-1                            deb   CVE-2023-4134     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2023-39191    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2023-31085    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2023-31081    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2023-26242    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2023-23039    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-45888    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-45885    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-45884    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-44034    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-44033    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-44032    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-41848    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-3238     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-2961     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-25265    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-1247     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2022-0400     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2021-3714     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2021-26934    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2020-35501    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2020-11725    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-19378    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-19070    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-16234    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-16233    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-16232    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-16231    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-16230    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-16229    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-12456    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-12455    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-12382    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-12381    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-12380    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-12379    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-12378    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2019-11191    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2018-17977    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2018-1121     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2017-13694    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2017-13693    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2017-0630     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2016-8660     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2016-10723    Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2015-2877     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2014-9900     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2014-9892     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2012-4542     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2011-4917     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2011-4916     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2011-4915     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2010-5321     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2010-4563     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2008-4609     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2008-2544     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2007-3719     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2005-3660     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2004-0230     Negligible  
linux-libc-dev             6.1.76-1                            deb   CVE-2024-25741    Unknown     
linux-libc-dev             6.1.76-1                            deb   CVE-2024-25740    Unknown     
linux-libc-dev             6.1.76-1                            deb   CVE-2024-25739    Unknown     
linux-libc-dev             6.1.76-1                            deb   CVE-2023-52429    Unknown     
login                      1:4.13+dfsg1-1+b1      (won't fix)  deb   CVE-2023-4641     Medium      
login                      1:4.13+dfsg1-1+b1      (won't fix)  deb   CVE-2023-29383    Low         
login                      1:4.13+dfsg1-1+b1                   deb   CVE-2019-19882    Negligible  
login                      1:4.13+dfsg1-1+b1                   deb   CVE-2007-5686     Negligible  
mount                      2.38.1-5+b1                         deb   CVE-2022-0563     Negligible  
ncurses-base               6.4-4                  (won't fix)  deb   CVE-2023-50495    Medium      
ncurses-bin                6.4-4                  (won't fix)  deb   CVE-2023-50495    Medium      
openssh-client             1:9.2p1-2+deb12u2      (won't fix)  deb   CVE-2023-51767    High        
openssh-client             1:9.2p1-2+deb12u2                   deb   CVE-2020-15778    Negligible  
openssh-client             1:9.2p1-2+deb12u2                   deb   CVE-2020-14145    Negligible  
openssh-client             1:9.2p1-2+deb12u2                   deb   CVE-2019-6110     Negligible  
openssh-client             1:9.2p1-2+deb12u2                   deb   CVE-2018-15919    Negligible  
openssh-client             1:9.2p1-2+deb12u2                   deb   CVE-2016-20012    Negligible  
openssh-client             1:9.2p1-2+deb12u2                   deb   CVE-2008-3234     Negligible  
openssh-client             1:9.2p1-2+deb12u2                   deb   CVE-2007-2768     Negligible  
openssh-client             1:9.2p1-2+deb12u2                   deb   CVE-2007-2243     Negligible  
openssl                    3.0.11-1~deb12u2       (won't fix)  deb   CVE-2024-0727     Medium      
openssl                    3.0.11-1~deb12u2       (won't fix)  deb   CVE-2023-6129     Medium      
openssl                    3.0.11-1~deb12u2       (won't fix)  deb   CVE-2023-5678     Medium      
openssl                    3.0.11-1~deb12u2                    deb   CVE-2010-0928     Negligible  
openssl                    3.0.11-1~deb12u2                    deb   CVE-2007-6755     Negligible  
openssl                    3.0.11-1~deb12u2       (won't fix)  deb   CVE-2023-6237     Unknown     
passwd                     1:4.13+dfsg1-1+b1      (won't fix)  deb   CVE-2023-4641     Medium      
passwd                     1:4.13+dfsg1-1+b1      (won't fix)  deb   CVE-2023-29383    Low         
passwd                     1:4.13+dfsg1-1+b1                   deb   CVE-2019-19882    Negligible  
passwd                     1:4.13+dfsg1-1+b1                   deb   CVE-2007-5686     Negligible  
perl                       5.36.0-7+deb12u1       (won't fix)  deb   CVE-2023-31484    High        
perl                       5.36.0-7+deb12u1                    deb   CVE-2023-31486    Negligible  
perl                       5.36.0-7+deb12u1           a0557@cve-bliss:santoshdts$ grype santoshdts/server:go
 ✔ Vulnerability DB                [no update available]  
 ✔ Loaded image                                                                                                                                                                                       santoshdts/server:go
 ✔ Parsed image                                                                                                                                    sha256:f0b736f8fb0a14652645df7b1a181790b4f25d8615ed70a884ff59c19c37a3aa
 ✔ Cataloged contents                                                                                                                                     f86a5fb1972dde8ff8a7e87c51cc578efc09490cd56cec2bc83a785a2be422de
   ├── ✔ Packages                        [249 packages]  
   ├── ✔ File digests                    [12,901 files]  
   ├── ✔ File metadata                   [12,901 locations]  
   └── ✔ Executables                     [1,069 executables]  
 ✔ Scanned for vulnerabilities     [358 vulnerability matches]  
   ├── by severity: 1 critical, 34 high, 81 medium, 8 low, 228 negligible (6 unknown)
   └── by status:   0 fixed, 358 not-fixed, 0 ignored 
[0009]  WARN cataloger failed cataloger=java-archive-cataloger error=unable to read files from java archive: unable to open zip archive (/tmp/syft-archive-contents-619634932/archive-test-badbase.zip): unable to open ZipR
[0009]  WARN cataloger failed cataloger=java-archive-cataloger error=unable to read files from java archive: unable to open zip archive (/tmp/syft-archive-contents-1997391525/archive-test-baddirsz.zip): unable to open Zi
[0010]  WARN cataloger failed cataloger=linux-kernel-cataloger error=unable to get magic type for file: EOF location=/usr/local/go/src/debug/pe/testdata/vmlinuz-4.15.0-47-generic
[0011]  WARN unable to process executable "/usr/local/go/src/debug/pe/testdata/vmlinuz-4.15.0-47-generic" error=unable to determine executable kind: unable to read enough bytes to determine executable format
NAME                       INSTALLED              FIXED-IN     TYPE  VULNERABILITY     SEVERITY   
apt                        2.6.1                               deb   CVE-2011-3374     Negligible  
binutils                   2.40-2                              deb   CVE-2023-1972     Negligible  
binutils                   2.40-2                              deb   CVE-2021-32256    Negligible  

<REDACTED>
.
.
util-linux-extra           2.38.1-5+b1                         deb   CVE-2022-0563     Negligible  
wget                       1.21.3-1+b2            (won't fix)  deb   CVE-2021-31879    Medium      
zlib1g                     1:1.2.13.dfsg-1        (won't fix)  deb   CVE-2023-45853    Critical         deb   CVE-2011-4116     Negligible  
perl-base                  5.36.0-7+deb12u1       (won't fix)  deb   CVE-2023-31484    High        
perl-base                  5.36.0-7+deb12u1                    deb   CVE-2023-31486    Negligible  
perl-base                  5.36.0-7+deb12u1                    deb   CVE-2011-4116     Negligible  
perl-modules-5.36          5.36.0-7+deb12u1       (won't fix)  deb   CVE-2023-31484    High        
perl-modules-5.36          5.36.0-7+deb12u1                    deb   CVE-2023-31486    Negligible  
perl-modules-5.36          5.36.0-7+deb12u1                    deb   CVE-2011-4116     Negligible  
procps                     2:4.0.2-3              (won't fix)  deb   CVE-2023-4016     Low         
python3.11                 3.11.2-6               (won't fix)  deb   CVE-2023-41105    High        
python3.11                 3.11.2-6               (won't fix)  deb   CVE-2023-24329    High        
python3.11                 3.11.2-6               (won't fix)  deb   CVE-2023-40217    Medium      
python3.11                 3.11.2-6               (won't fix)  deb   CVE-2023-27043    Medium      
python3.11                 3.11.2-6                            deb   CVE-2023-24535    Negligible  
python3.11-minimal         3.11.2-6               (won't fix)  deb   CVE-2023-41105    High        
python3.11-minimal         3.11.2-6               (won't fix)  deb   CVE-2023-24329    High        
python3.11-minimal         3.11.2-6               (won't fix)  deb   CVE-2023-40217    Medium      
python3.11-minimal         3.11.2-6               (won't fix)  deb   CVE-2023-27043    Medium      
python3.11-minimal         3.11.2-6                            deb   CVE-2023-24535    Negligible  
tar                        1.34+dfsg-1.2+deb12u1               deb   CVE-2005-2541     Negligible  
util-linux                 2.38.1-5+b1                         deb   CVE-2022-0563     Negligible  
util-linux-extra           2.38.1-5+b1                         deb   CVE-2022-0563     Negligible  
wget                       1.21.3-1+b2            (won't fix)  deb   CVE-2021-31879    Medium      
zlib1g                     1:1.2.13.dfsg-1        (won't fix)  deb   CVE-2023-45853    Critical
```

## Chainguaard-Golang-server

```shell
a0557@cve-bliss:santoshdts$ grype santoshdts/server:go-cgr
 ✔ Vulnerability DB                [no update available]  
 ✔ Loaded image                                                                                                                                                                                   santoshdts/server:go-cgr
 ✔ Parsed image                                                                                                                                    sha256:fe005ab96e25286da29b8d2d4e9b2699907c66928fd60f3896ed0e0ff4051cbd
 ✔ Cataloged contents                                                                                                                                     553f5bdc0519a69623d3cac9190255057e5c887aab26c3b8ea99a013573cfde8
   ├── ✔ Packages                        [100 packages]  
   ├── ✔ File digests                    [8,734 files]  
   ├── ✔ File metadata                   [8,734 locations]  
   └── ✔ Executables                     [213 executables]  
 ✔ Scanned for vulnerabilities     [0 vulnerability matches]  
   ├── by severity: 0 critical, 0 high, 0 medium, 0 low, 0 negligible
   └── by status:   0 fixed, 0 not-fixed, 0 ignored 
No vulnerabilities found
```