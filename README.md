# Singularity Picard

This will produce a Singularity image (suitable for running in a cluster environment) using [https://hub.docker.com/r/broadinstitute/picard/](https://hub.docker.com/r/broadinstitute/picard/). We do this by way of a bootstrap file for the Docker image.


## 1. Install Singularity

Instructions can be found on the [singularity site](https://singularityware.github.io).


## 2. Bootstrap the image


    sudo singularity create --size 4000 picard.img
    sudo singularity bootstrap picard.img Singularity


## 3. Run commands

How to access the picard runtime executable?


      ./picard.img -h
