# BOSS TONE STUDIO for Linux 🎸🐧

An unofficial port of BOSS TONE STUDIO to Linux.

## Installing

### Requirements

1. Docker Engine for Linux: https://docs.docker.com/engine/install/
2. Make sure [docker buildx](https://docs.docker.com/reference/cli/docker/buildx/) (BuildKit) is installed, or you can't export the binary

### Building

To build the application and place the resulting packages (.deb, .rpm, .AppImage) in a directory named `out/`, run:

```
docker build . -f Dockerfile.prepare -o . && docker build . -o out
```

The resulting packages can be directly installed with your distribution's package manager.

## Developing

### Requirements

1. Tauri Prerequisites: https://v2.tauri.app/start/prerequisites/

### Preparation

To prepare the repository for development:

```
docker build . -f Dockerfile.prepare -o .
cd tauri
npm install
```

### Running

```
cd tauri
npm run tauri dev
```

## Supported BOSS TONE STUDIO Versions

| Version                                     | Status | Notes                                 |
| ------------------------------------------- | ------ | ------------------------------------- |
| BOSS TONE STUDIO for KATANA Gen 3 Ver 1.1.0 | 🚧      | All controls that I have tested work. |
