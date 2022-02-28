# Euroargodev shared environment for Binder service

Use this repo to speed up Binder launches by pulling your github content in a Binder link with nbgitpuller.

This repo is here to de-couple the content of your euroargodev repository you want to run Binder on, from the environment that is needed to run it.

To generate your "Open with Binder" links, please check: https://euroargodev.github.io/binder-links-creator/

## Example

[![Binder](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Binder&message=Open+argopy+demo&color=blue)](https://mybinder.org/v2/gh/euroargodev/binder-sandbox/main?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Feuroargodev%252Fargopy%26urlpath%3Dlab%252Ftree%252Fargopy%252Fdocs%252Ftryit.ipynb%26branch%3Dmaster)

## Environment
Binder jupyterhub instances are created using the following Pangeo docker images:

| branch | Pangeo image |
|:---------:|:-------|
| main | pangeo/pangeo-notebook:latest, [open env. here](https://github.com/pangeo-data/pangeo-docker-images/blob/master/pangeo-notebook/environment.yml) | 

List of images:
https://hub.docker.com/u/pangeo

More on Pangeo images:
https://github.com/pangeo-data/pangeo-docker-images