# Oceta OS

## Installation

Installing docker image from Docker File

```bash
docker build buildenv -t oceta-buildenv
```

Running an instance of docker image

Linux or Mac:

```bash
docker run --rm -it -v $(pwd):/root/env oceta-buildenv
```

Windows:

CMD:

```bash
docker run --rm -it -v "%cd%":/root/env oceta-buildenv
```
Powershell:

```bash
docker run --rm -it -v "${pwd}:/root/env" oceta-buildenv
```

## Building the files

```bash
make build-x86_64
```

## Running the Qemu

```bash
qemu-system-x86_64 -cdrom /dist/x86_64/kernel.iso
```
