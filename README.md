# Euroargodev software environments for Binder service

This repo is here to **de-couple the content of your euroargodev repository from the environment that is needed to run it on Binder**.

To generate your "Open with Binder" links, please check: https://euroargodev.github.io/binder-links-creator/

Use this repo to:
1. avoid the pain of setting up a customised Binder on your repo (use this repo branches instead)
2. speed up Binder launch from your repo (de-couple content from environment)

## Examples

[![Binder](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Binder&message=Open+argopy+demo&color=blue)](https://mybinder.org/v2/gh/euroargodev/binder-sandbox/main?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Feuroargodev%252Fargopy%26urlpath%3Dlab%252Ftree%252Fargopy%252Fdocs%252Ftryit.ipynb%26branch%3Dmaster)

[![Binder](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Binder&message=Open+OSnet+demo&color=blue)](https://mybinder.org/v2/gh/euroargodev/binder-sandbox/pangeo-ml?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Feuroargodev%252FOSnet-GulfStream%26urlpath%3Dlab%252Ftree%252FOSnet-GulfStream%252Fdocs%252Fdemo-predictions.ipynb%26branch%3Dbinder)

## Environments
Binder jupyterhub instances are created using the following Pangeo docker images:

| branch | Pangeo image | Euroargodev additionnal packages |
|:---------:|:-------|:-------|
| main | pangeo/pangeo-notebook:latest, [see env. here](https://github.com/pangeo-data/pangeo-docker-images/tree/master/ml-notebook) | cmocean, argopy
| pangeo-ml | pangeo/ml-notebook:latest, [see env. here](https://github.com/pangeo-data/pangeo-docker-images/tree/master/ml-notebook) | cmocean, argopy

## Contribute 
If you want to add a new package:
- [ ] fork this repo,
- [ ] select the branch you want to update, 
- [ ] make your changes in the Dockerfile and README.md files, 
- [ ] make a PR.

## More resources:
List of Pangeo images: https://hub.docker.com/u/pangeo

Source code for Pangeo images: https://github.com/pangeo-data/pangeo-docker-images

More on Pangeo cloud software environments: https://pangeo.io/cloud#software-environment

How to customise Binder build: https://mybinder.readthedocs.io/en/latest/tutorials/dockerfile.html