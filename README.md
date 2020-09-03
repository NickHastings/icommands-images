# icommands-images
Definition files to create Singularity images with the iRODs icommands installed.

## Usage

A Singularity image file based on Ubuntu 18.04 with the icommands can be created with the command:
```
singularity build Ubuntu1804-icommands.sif Ubuntu1804-icommands.def
```

The image can then be used to run commands like `ils`, `iget`, `iput` etc provided the user has a valid `~/.irods/` setup on the host machine:
```
singularity exec Ubuntu1804-icommands.sif ils                 
```
