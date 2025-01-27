grype docker:sherlocknocg                                 
 ✔ Vulnerability DB                [updated]  
 ✔ Loaded image                                                                                                                                    sherlocknocg:latest
 ✔ Parsed image                                                                                sha256:c1191d29a9a143d188b2b86e0963fb47624603ac9693c5c70c468852c0fcbec4
 ✔ Cataloged contents                                                                                 b478412cf1ef8cfc17626af60d5e95d77fb44619c4ef0036b936dcd105f42f0b
   ├── ✔ Packages                        [134 packages]  
   ├── ✔ File digests                    [3,372 files]  
   └── ✔ File metadata                   [3,372 locations]  
 ✔ Scanned for vulnerabilities     [135 vulnerability matches]  
   ├── by severity: 2 critical, 17 high, 26 medium, 7 low, 64 negligible (19 unknown)
   └── by status:   0 fixed, 135 not-fixed, 0 ignored 
NAME                INSTALLED                FIXED-IN     TYPE  VULNERABILITY     SEVERITY   
apt                 2.2.4                                 deb   CVE-2011-3374     Negligible  
bash                5.1-2+deb11u1            (won't fix)  deb   CVE-2022-3715     High        
bsdutils            1:2.36.1-8+deb11u1                    deb   CVE-2022-0563     Negligible  
coreutils           8.32-4                   (won't fix)  deb   CVE-2016-2781     Low         
coreutils           8.32-4                                deb   CVE-2017-18018    Negligible  
e2fsprogs           1.46.2-2                 (won't fix)  deb   CVE-2022-1304     High        
gcc-10-base         10.2.1-6                 (won't fix)  deb   CVE-2023-4039     Medium      
gcc-9-base          9.3.0-22                 (won't fix)  deb   CVE-2023-4039     Medium      
gpgv                2.2.27-2+deb11u2                      deb   CVE-2022-3219     Negligible  
libapt-pkg6.0       2.2.4                                 deb   CVE-2011-3374     Negligible  
libblkid1           2.36.1-8+deb11u1                      deb   CVE-2022-0563     Negligible  
libc-bin            2.31-13+deb11u8          (won't fix)  deb   CVE-2023-4813     Medium      
libc-bin            2.31-13+deb11u8          (won't fix)  deb   CVE-2023-4806     Medium      
libc-bin            2.31-13+deb11u8                       deb   CVE-2019-9192     Negligible  
libc-bin            2.31-13+deb11u8                       deb   CVE-2019-1010025  Negligible  
libc-bin            2.31-13+deb11u8                       deb   CVE-2019-1010024  Negligible  
libc-bin            2.31-13+deb11u8                       deb   CVE-2019-1010023  Negligible  
libc-bin            2.31-13+deb11u8                       deb   CVE-2019-1010022  Negligible  
libc-bin            2.31-13+deb11u8                       deb   CVE-2018-20796    Negligible  
libc-bin            2.31-13+deb11u8                       deb   CVE-2010-4756     Negligible  
libc6               2.31-13+deb11u8          (won't fix)  deb   CVE-2023-4813     Medium      
libc6               2.31-13+deb11u8          (won't fix)  deb   CVE-2023-4806     Medium      
libc6               2.31-13+deb11u8                       deb   CVE-2019-9192     Negligible  
libc6               2.31-13+deb11u8                       deb   CVE-2019-1010025  Negligible  
libc6               2.31-13+deb11u8                       deb   CVE-2019-1010024  Negligible  
libc6               2.31-13+deb11u8                       deb   CVE-2019-1010023  Negligible  
libc6               2.31-13+deb11u8                       deb   CVE-2019-1010022  Negligible  
libc6               2.31-13+deb11u8                       deb   CVE-2018-20796    Negligible  
libc6               2.31-13+deb11u8                       deb   CVE-2010-4756     Negligible  
libcom-err2         1.46.2-2                 (won't fix)  deb   CVE-2022-1304     High        
libdb5.3            5.3.28+dfsg1-0.8         (won't fix)  deb   CVE-2019-8457     Critical    
libexpat1           2.2.10-2+deb11u5                      deb   CVE-2023-52425    High        
libexpat1           2.2.10-2+deb11u5                      deb   CVE-2023-52426    Medium      
libexpat1           2.2.10-2+deb11u5                      deb   CVE-2013-0340     Negligible  
libexpat1           2.2.10-2+deb11u5                      deb   CVE-2024-28757    Unknown     
libext2fs2          1.46.2-2                 (won't fix)  deb   CVE-2022-1304     High        
libgcc-s1           10.2.1-6                 (won't fix)  deb   CVE-2023-4039     Medium      
libgcrypt20         1.8.7-6                  (won't fix)  deb   CVE-2021-33560    High        
libgcrypt20         1.8.7-6                  (won't fix)  deb   CVE-2024-2236     Medium      
libgcrypt20         1.8.7-6                               deb   CVE-2018-6829     Negligible  
libgnutls30         3.7.1-5+deb11u4          (won't fix)  deb   CVE-2024-0567     High        
libgnutls30         3.7.1-5+deb11u4          (won't fix)  deb   CVE-2024-0553     High        
libgnutls30         3.7.1-5+deb11u4                       deb   CVE-2011-3389     Negligible  
libgssapi-krb5-2    1.18.3-6+deb11u4                      deb   CVE-2018-5709     Negligible  
libgssapi-krb5-2    1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26462    Unknown     
libgssapi-krb5-2    1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26461    Unknown     
libgssapi-krb5-2    1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26458    Unknown     
libk5crypto3        1.18.3-6+deb11u4                      deb   CVE-2018-5709     Negligible  
libk5crypto3        1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26462    Unknown     
libk5crypto3        1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26461    Unknown     
libk5crypto3        1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26458    Unknown     
libkrb5-3           1.18.3-6+deb11u4                      deb   CVE-2018-5709     Negligible  
libkrb5-3           1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26462    Unknown     
libkrb5-3           1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26461    Unknown     
libkrb5-3           1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26458    Unknown     
libkrb5support0     1.18.3-6+deb11u4                      deb   CVE-2018-5709     Negligible  
libkrb5support0     1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26462    Unknown     
libkrb5support0     1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26461    Unknown     
libkrb5support0     1.18.3-6+deb11u4         (won't fix)  deb   CVE-2024-26458    Unknown     
libmount1           2.36.1-8+deb11u1                      deb   CVE-2022-0563     Negligible  
libncursesw6        6.2+20201114-2+deb11u2   (won't fix)  deb   CVE-2023-50495    Medium      
libncursesw6        6.2+20201114-2+deb11u2   (won't fix)  deb   CVE-2023-45918    Unknown     
libpam-modules      1.4.0-9+deb11u1          (won't fix)  deb   CVE-2024-22365    Medium      
libpam-modules-bin  1.4.0-9+deb11u1          (won't fix)  deb   CVE-2024-22365    Medium      
libpam-runtime      1.4.0-9+deb11u1          (won't fix)  deb   CVE-2024-22365    Medium      
libpam0g            1.4.0-9+deb11u1          (won't fix)  deb   CVE-2024-22365    Medium      
libpcre2-8-0        10.36-2+deb11u1                       deb   CVE-2022-41409    Negligible  
libpcre3            2:8.39-13                             deb   CVE-2019-20838    Negligible  
libpcre3            2:8.39-13                             deb   CVE-2017-7246     Negligible  
libpcre3            2:8.39-13                             deb   CVE-2017-7245     Negligible  
libpcre3            2:8.39-13                             deb   CVE-2017-16231    Negligible  
libpcre3            2:8.39-13                             deb   CVE-2017-11164    Negligible  
libsepol1           3.1-1                    (won't fix)  deb   CVE-2021-36087    Low         
libsepol1           3.1-1                    (won't fix)  deb   CVE-2021-36086    Low         
libsepol1           3.1-1                    (won't fix)  deb   CVE-2021-36085    Low         
libsepol1           3.1-1                    (won't fix)  deb   CVE-2021-36084    Low         
libsmartcols1       2.36.1-8+deb11u1                      deb   CVE-2022-0563     Negligible  
libsqlite3-0        3.34.1-3                 (won't fix)  deb   CVE-2023-7104     High        
libsqlite3-0        3.34.1-3                 (won't fix)  deb   CVE-2021-31239    High        
libsqlite3-0        3.34.1-3                              deb   CVE-2022-35737    Negligible  
libsqlite3-0        3.34.1-3                              deb   CVE-2021-45346    Negligible  
libsqlite3-0        3.34.1-3                              deb   CVE-2021-36690    Negligible  
libss2              1.46.2-2                 (won't fix)  deb   CVE-2022-1304     High        
libssl1.1           1.1.1w-0+deb11u1         (won't fix)  deb   CVE-2024-0727     Medium      
libssl1.1           1.1.1w-0+deb11u1         (won't fix)  deb   CVE-2023-5678     Medium      
libssl1.1           1.1.1w-0+deb11u1                      deb   CVE-2010-0928     Negligible  
libssl1.1           1.1.1w-0+deb11u1                      deb   CVE-2007-6755     Negligible  
libstdc++6          10.2.1-6                 (won't fix)  deb   CVE-2023-4039     Medium      
libsystemd0         247.3-7+deb11u4          (won't fix)  deb   CVE-2023-50387    High        
libsystemd0         247.3-7+deb11u4          (won't fix)  deb   CVE-2023-7008     Medium      
libsystemd0         247.3-7+deb11u4                       deb   CVE-2023-31439    Negligible  
libsystemd0         247.3-7+deb11u4                       deb   CVE-2023-31438    Negligible  
libsystemd0         247.3-7+deb11u4                       deb   CVE-2023-31437    Negligible  
libsystemd0         247.3-7+deb11u4                       deb   CVE-2020-13529    Negligible  
libsystemd0         247.3-7+deb11u4                       deb   CVE-2013-4392     Negligible  
libsystemd0         247.3-7+deb11u4          (won't fix)  deb   CVE-2023-50868    Unknown     
libtinfo6           6.2+20201114-2+deb11u2   (won't fix)  deb   CVE-2023-50495    Medium      
libtinfo6           6.2+20201114-2+deb11u2   (won't fix)  deb   CVE-2023-45918    Unknown     
libudev1            247.3-7+deb11u4          (won't fix)  deb   CVE-2023-50387    High        
libudev1            247.3-7+deb11u4          (won't fix)  deb   CVE-2023-7008     Medium      
libudev1            247.3-7+deb11u4                       deb   CVE-2023-31439    Negligible  
libudev1            247.3-7+deb11u4                       deb   CVE-2023-31438    Negligible  
libudev1            247.3-7+deb11u4                       deb   CVE-2023-31437    Negligible  
libudev1            247.3-7+deb11u4                       deb   CVE-2020-13529    Negligible  
libudev1            247.3-7+deb11u4                       deb   CVE-2013-4392     Negligible  
libudev1            247.3-7+deb11u4          (won't fix)  deb   CVE-2023-50868    Unknown     
libuuid1            2.36.1-8+deb11u1                      deb   CVE-2022-0563     Negligible  
libzstd1            1.4.8+dfsg-2.1           (won't fix)  deb   CVE-2022-4899     High        
login               1:4.8.1-1                (won't fix)  deb   CVE-2023-4641     Medium      
login               1:4.8.1-1                (won't fix)  deb   CVE-2023-29383    Low         
login               1:4.8.1-1                             deb   CVE-2019-19882    Negligible  
login               1:4.8.1-1                             deb   CVE-2013-4235     Negligible  
login               1:4.8.1-1                             deb   CVE-2007-5686     Negligible  
logsave             1.46.2-2                 (won't fix)  deb   CVE-2022-1304     High        
mount               2.36.1-8+deb11u1                      deb   CVE-2022-0563     Negligible  
ncurses-base        6.2+20201114-2+deb11u2   (won't fix)  deb   CVE-2023-50495    Medium      
ncurses-base        6.2+20201114-2+deb11u2   (won't fix)  deb   CVE-2023-45918    Unknown     
ncurses-bin         6.2+20201114-2+deb11u2   (won't fix)  deb   CVE-2023-50495    Medium      
ncurses-bin         6.2+20201114-2+deb11u2   (won't fix)  deb   CVE-2023-45918    Unknown     
openssl             1.1.1w-0+deb11u1         (won't fix)  deb   CVE-2024-0727     Medium      
openssl             1.1.1w-0+deb11u1         (won't fix)  deb   CVE-2023-5678     Medium      
openssl             1.1.1w-0+deb11u1                      deb   CVE-2010-0928     Negligible  
openssl             1.1.1w-0+deb11u1                      deb   CVE-2007-6755     Negligible  
passwd              1:4.8.1-1                (won't fix)  deb   CVE-2023-4641     Medium      
passwd              1:4.8.1-1                (won't fix)  deb   CVE-2023-29383    Low         
passwd              1:4.8.1-1                             deb   CVE-2019-19882    Negligible  
passwd              1:4.8.1-1                             deb   CVE-2013-4235     Negligible  
passwd              1:4.8.1-1                             deb   CVE-2007-5686     Negligible  
perl-base           5.32.1-4+deb11u3         (won't fix)  deb   CVE-2023-31484    High        
perl-base           5.32.1-4+deb11u3         (won't fix)  deb   CVE-2020-16156    High        
perl-base           5.32.1-4+deb11u3                      deb   CVE-2023-31486    Negligible  
perl-base           5.32.1-4+deb11u3                      deb   CVE-2011-4116     Negligible  
tar                 1.34+dfsg-1+deb11u1                   deb   CVE-2005-2541     Negligible  
util-linux          2.36.1-8+deb11u1                      deb   CVE-2022-0563     Negligible  
zlib1g              1:1.2.11.dfsg-2+deb11u2  (won't fix)  deb   CVE-2023-45853    Critical



grype docker:sherlockcg                         
 ✔ Vulnerability DB                [no update available]  
 ✔ Loaded image                                                                                                                                      sherlockcg:latest
 ✔ Parsed image                                                                                sha256:4e0222e537eed336faaa1685e1022e05e2a651301a6fbf7c8b35d98eecfd7d3d
 ✔ Cataloged contents                                                                                 8ac7d5b1c8e8aaaf80982b707abd7e69b854f419f42423223b51a405fc7ed09c
   ├── ✔ Packages                        [85 packages]  
   ├── ✔ File digests                    [7,207 files]  
   └── ✔ File metadata                   [7,207 locations]  
 ✔ Scanned for vulnerabilities     [0 vulnerability matches]  
   ├── by severity: 0 critical, 0 high, 0 medium, 0 low, 0 negligible
   └── by status:   0 fixed, 0 not-fixed, 0 ignored 
No vulnerabilities found

