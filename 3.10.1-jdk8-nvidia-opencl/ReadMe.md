DOCKER_BUILDKIT=1 docker build  --no-cache \
--build-arg GDAL_BUILD_IS_RELEASE=YES \
-t fsystem/gdal:3.10.1-jdk8-nvidia-opencl .