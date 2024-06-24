# GDAL

GDAL Java Tomcat JDK filegdb

## RUN

for tag `3.9-jdk8` `3.9-jdk17` `3.9-jdk21` `3.9-jdk8` `v3.0.0-openj9`

```

ENTRYPOINT ["/bin/sh", "-c","for jar in /jars/*.jar; do java $JAVA_OPTS -jar $jar; done"]
```

## Introduction

Tag `base` is enviroment used for building gdal.
Other tag are production with gdal inside.
Failed many times when I build gdal with ESRI FileGeodatabaseAPI_1.5.1 based on Alpine Linux, as FileGeodatabaseAPI depends on glibc, and Alpine Linux is packaged with musl libc.  
So I switch to Debian based Docker images,  and finally I went throuth it.

## Version Info

| tag | gdal | tomcat | jdk | os | fgdb |
| - | - | - | - | - | - |
| 3.9-jdk8 | 3.9.0 | none | amazoncrectto jdk8 | Alpine 3.20 | none |
| 3.9-jdk17 | 3.9.0 | none | amazoncrectto jdk17 | Alpine 3.20 | none |
| 3.9-jdk21 | 3.9.0 |  none | amazoncrectto jdk21| Alpine 3.320 | none |
| base | none | 8.5 | open jdk 8 | Alpine 3.3 | none |
| base-debian | none | 8.5 | open jdk 8 | Debian 9 | none |
| v2.2.0-tomcat | v2.2.0 | 8.5 | open jdk 8 | Alpine 3.39 | none |
| v3.0.0-tomcat | v3.0.0 | 8.5 | open jdk 8 | Debian 9 | 1.5.1 |
| v3.0.0-openj9 | v3.0.0 | none | open jdk 8 | Ubuntu 18 | 1.5.1 |
