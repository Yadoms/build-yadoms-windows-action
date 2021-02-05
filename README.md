# build-yadoms-windows-action github action

This action allow to generate a yadoms build for **Windows** using Github Actions.

## Inputs


### `buildImage`

**required** The image to use for building Yadoms. 

### `registry`

*optional* The registry where to pull image (default : ''). 

### `username`

*optional* The registry username (default : '')

### `password`

*optional* The registry password (default : '')

### `privileged`

*optional* To run the container in privileged mode, set this input to "--privileged"

### `entrypoint`

*optional* The entrypoint override (default : C:\entrypoint_docker.cmd)

### `param1`, `param2`, `param3`, `param4`

*optional* Free parameters passed to docker container

## Outputs

### `yadomsVersion`

The current building yadoms full version, example : '2.5.0-beta.1'

## Example usage

- name: Yadoms build script
  uses: Yadoms/build-yadoms-windows-action@v2.0.0
  
