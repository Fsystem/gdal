FROM tomcat:8.5-jdk8-openjdk

MAINTAINER haies 

RUN apt-get update -y \
    && apt-get install -y --fix-missing --no-install-recommends \
            software-properties-common build-essential ca-certificates \
            git make cmake wget unzip libtool automake \
            zlib1g-dev libsqlite3-dev pkg-config sqlite3 \
            python3-dev python3-numpy \
            libjpeg-dev libgeos-dev \
            curl libcurl4-gnutls-dev libexpat-dev libxerces-c-dev \
            libwebp-dev \
            libzstd1-dev bash zip curl \
            libpq-dev libssl-dev \
            autoconf automake sqlite3 bash-completion \
            rsync ccache
