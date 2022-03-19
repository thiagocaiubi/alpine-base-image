alpine-base-image
========================

This repository contains the sources for the following [docker](https://docker.io) base images:
- [`thiagocaiubi/alpine-base-image`]

## Usage

This Image is intedend to be used in multi stage docker builds and is for final or production use.

```
FROM thiagocaiubi/alpine-base-image

ADD binfile /opt/test/binfile
WORKDIR /opt/test/

CMD binfile
```

## Developing and testing

```bash
# Pull image
git clone ssh://git@github.com/thiagocaiubi/alpine-base-image.git
cd alpine-base-image

# hack hack hack

# Build
make build
