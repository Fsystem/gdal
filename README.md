# GDAL

GDAL Java Tomcat JDK filegdb

## Introduction

Tag `base` is enviroment used for building gdal.
Other tag are production with gdal inside.
Failed many times when I build gdal with ESRI FileGeodatabaseAPI_1.5.1 based on Alpine Linux, as FileGeodatabaseAPI depends on glibc, and Alpine Linux is packaged with musl libc.  
So I switch to Debian based Docker images,  and finally I went throuth it.

## Version Info

| tag | gdal | tomcat | jdk | os | fgdb |
| - | - | - | - | - | - |
| base | none | 8.5 | open jdk 8 | Alpine 3.39 | none |
| base-debian | none | 8.5 | open jdk 8 | Debian 9 | none |
| v2.2.0-tomcat | v2.2.0 | 8.5 | open jdk 8 | Alpine 3.39 | none |
| v3.0.0-tomcat | v3.0.0 | 8.5 | open jdk 8 | Debian 9 | 1.5.1 |
| v3.0.0-openj9 | v3.0.0 | none | open jdk 8 | Ubuntu 18 | 1.5.1 |
