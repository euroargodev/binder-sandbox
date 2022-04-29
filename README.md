# Euroargodev software environments for Binder service

This repo is here to **de-couple the content of your euroargodev repository from the environment that is needed to run it on Binder**.

This repo allows to:
1. avoid the pain of setting up a customised Binder on your repo (use this repo branches instead)
2. speed up Binder launch from your repo (de-couple content from environment)

To generate your own "Open with Binder" links and badges, please check: https://euroargodev.github.io/binder-links-creator/

## Examples

[![Binder](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Binder&message=Open+argopy+demo&color=blue)](https://mybinder.org/v2/gh/euroargodev/binder-sandbox/main?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Feuroargodev%252Fargopy%26urlpath%3Dlab%252Ftree%252Fargopy%252Fdocs%252Ftryit.ipynb%26branch%3Dmaster)

[![Binder](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Binder&message=Open+OSnet+demo&color=blue)](https://mybinder.org/v2/gh/euroargodev/binder-sandbox/pangeo-ml?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Feuroargodev%252FOSnet-GulfStream%26urlpath%3Dlab%252Ftree%252FOSnet-GulfStream%252Fdocs%252Fdemo-predictions.ipynb%26branch%3Dbinder)

If you still want to set-up Binder in your own repo, just use this one as a template by [clicking here](https://github.com/euroargodev/binder-sandbox/generate) !

## Environments
Euroargodev Binder jupyterhub instances are created using the following Pangeo docker images:

| branch | Pangeo image | Euroargodev additional packages |
|:---------:|:-------|:-------|
| main | pangeo/pangeo-notebook:latest, <br>[see env. here](https://github.com/pangeo-data/pangeo-docker-images/tree/master/pangeo-notebook/environment.yml) | [cmocean](https://matplotlib.org/cmocean/)
| pangeo-ml | pangeo/ml-notebook:latest, [see env. here](https://github.com/pangeo-data/pangeo-docker-images/tree/master/ml-notebook/environment.yml) | [cmocean](https://matplotlib.org/cmocean/)
| virtual-fleet | pangeo/pangeo-notebook:latest, [see env. here](https://github.com/pangeo-data/pangeo-docker-images/tree/master/ml-notebook/environment.yml) | [cmocean](https://matplotlib.org/cmocean/), cgen, pymbolic, progressbar, [parcels](https://github.com/OceanParcels/parcels)

All Pangeo images [come with argopy installed](https://github.com/pangeo-data/pangeo-docker-images/pull/307).

## Customise 

The simple way: simply raise an issue to ask for a missing package !

The more complex way:
- [ ] fork this repo,
- [ ] select the branch you want to update, or create a new one, 
- [ ] make your changes in the Dockerfile and README.md files, 
- [ ] make a PR.

## More resources:
List of Pangeo images: https://hub.docker.com/u/pangeo

Source code for Pangeo images: https://github.com/pangeo-data/pangeo-docker-images

More on Pangeo cloud software environments: https://pangeo.io/cloud#software-environment

How to customise Binder build: https://repo2docker.readthedocs.io/en/latest/config_files.html

More on Dockerfile used by Binder: https://mybinder.readthedocs.io/en/latest/tutorials/dockerfile.html
