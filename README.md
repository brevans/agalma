# Singularity & agalma

This [singularity](http://singularity.lbl.gov/) definition file is meant to closely mirror the dockerfile for agalma. Singularity containers are well suited for running docker-like workflows in multi-user contexts, such as HPC clusters. Please see the [linux](http://singularity.lbl.gov/install-linux) or [MacOS](http://singularity.lbl.gov/install-mac) install instructions to get singularity.

To build this Singularity image:

```
sudo $(which singularity) build agalma.simg Singularity.latest
```

To pull this Singularity image from singularity-hub and run the agalma tests in current directory:
```
singularity run shub://brevans/agalma:latest
```
