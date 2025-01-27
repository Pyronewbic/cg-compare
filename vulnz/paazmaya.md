# Visual Regression Tracker: Frontend - Vulnerability comparison

> 2024-02-19, @paazmaya

## Original nginx-alpine-slim

The original Dockerfile uses `nginx:1.25-alpine3.17-slim` at
https://github.com/Visual-Regression-Tracker/frontend/blob/master/Dockerfile
which is used in the resulting image.

```
✔ Cataloged contents
  ├── ✔ Packages                        [19 packages]
  ├── ✔ File digests                    [803 files]
  ├── ✔ File metadata                   [803 locations]
  └── ✔ Executables                     [23 executables]
✔ Scanned for vulnerabilities     [10 vulnerability matches]
  ├── by severity: 0 critical, 2 high, 6 medium, 0 low, 0 negligible (2 unknown)
  └── by status:   10 fixed, 0 not-fixed, 0 ignored

NAME        INSTALLED  FIXED-IN   TYPE  VULNERABILITY  SEVERITY 
libcrypto3  3.0.10-r0  3.0.12-r0  apk   CVE-2023-5363  High      
libcrypto3  3.0.10-r0  3.0.12-r4  apk   CVE-2024-0727  Medium    
libcrypto3  3.0.10-r0  3.0.12-r2  apk   CVE-2023-6129  Medium    
libcrypto3  3.0.10-r0  3.0.12-r1  apk   CVE-2023-5678  Medium    
libcrypto3  3.0.10-r0  3.0.12-r3  apk   CVE-2023-6237  Unknown   
libssl3     3.0.10-r0  3.0.12-r0  apk   CVE-2023-5363  High      
libssl3     3.0.10-r0  3.0.12-r4  apk   CVE-2024-0727  Medium    
libssl3     3.0.10-r0  3.0.12-r2  apk   CVE-2023-6129  Medium    
libssl3     3.0.10-r0  3.0.12-r1  apk   CVE-2023-5678  Medium    
libssl3     3.0.10-r0  3.0.12-r3  apk   CVE-2023-6237  Unknown
```

## More recent version of Alpine

Taking a more recent version of Alpine in use with `nginx:1.25-alpine3.18-slim` image.

```
✔ Cataloged contents
  ├── ✔ Packages                        [19 packages]
  ├── ✔ File digests                    [806 files]
  ├── ✔ File metadata                   [806 locations]
  └── ✔ Executables                     [23 executables]
✔ Scanned for vulnerabilities     [12 vulnerability matches]
  ├── by severity: 0 critical, 0 high, 12 medium, 0 low, 0 negligible
  └── by status:   0 fixed, 12 not-fixed, 0 ignored

NAME           INSTALLED  FIXED-IN  TYPE  VULNERABILITY   SEVERITY
busybox        1.36.1-r5            apk   CVE-2023-42366  Medium
busybox        1.36.1-r5            apk   CVE-2023-42365  Medium
busybox        1.36.1-r5            apk   CVE-2023-42364  Medium
busybox        1.36.1-r5            apk   CVE-2023-42363  Medium
busybox-binsh  1.36.1-r5            apk   CVE-2023-42366  Medium
busybox-binsh  1.36.1-r5            apk   CVE-2023-42365  Medium
busybox-binsh  1.36.1-r5            apk   CVE-2023-42364  Medium
busybox-binsh  1.36.1-r5            apk   CVE-2023-42363  Medium
ssl_client     1.36.1-r5            apk   CVE-2023-42366  Medium
ssl_client     1.36.1-r5            apk   CVE-2023-42365  Medium
ssl_client     1.36.1-r5            apk   CVE-2023-42364  Medium
ssl_client     1.36.1-r5            apk   CVE-2023-42363  Medium
```

## Moved to chainguard-nginx

Moving to use `cgr.dev/chainguard/nginx:latest` in the resulting image.

```
✔ Cataloged contents
  ├── ✔ Packages                        [16 packages]
  ├── ✔ File digests                    [172 files]
  ├── ✔ File metadata                   [172 locations]
  └── ✔ Executables                     [34 executables]
✔ Scanned for vulnerabilities     [0 vulnerability matches]
  ├── by severity: 0 critical, 0 high, 0 medium, 0 low, 0 negligible
  └── by status:   0 fixed, 0 not-fixed, 0 ignored

No vulnerabilities found
```
