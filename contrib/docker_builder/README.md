# Dockerfile for building indicoin binaries.

Now, you can build your own indicoin files on all systems with docker and do it easy without installing depends on your system.

## How:

### Build docker image

```
sudo docker build .
```

### Run docker container

Builder will return HASH of image
Example:
Successfully built 9bbff825d50f

```
sudo docker run -it -v ~/path/to/indicoin/folder:/indicoin 9bbff825d50f
```

If your system uses SELINUX you may use --privileged=true key

```
sudo docker run --privileged=true -it -v ~/development/indicoin:/indicoin 9bbff825d50f
```

See indicoin-qt file in used indicoin folder and indicoind file in src subfolder.