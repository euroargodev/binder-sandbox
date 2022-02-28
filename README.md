# Sandbox for Binder service at euroargodev

Use this repo to speed up Binder launches by pulling your github content in a Binder link with nbgitpuller.

This repo is here to de-couple the content of your euroargodev repository you want to run Binder on, from the environment that is needed to run it.

For mode advanced link generator, please check: https://jupyterhub.github.io/nbgitpuller/link

https://mybinder.org/v2/gh/euroargodev/binder-sandbox/main?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Feuroargodev%252FOSnet-GulfStream%26urlpath%3Dlab%252Ftree%252FOSnet-GulfStream%252Fdocs%252Fdemo-predictions.ipynb%26branch%3Dbinder


Git Environment Repository URL: https://github.com/euroargodev/binder-sandbox

Git Content URL: https://github.com/euroargodev/OSnet-GulfStream

Examples:

Launch Binder with classic jupyter notebooks at your root repo level:
https://mybinder.org/v2/gh/euroargodev/binder-sandbox/main?urlpath=git-pull?repo=https://github.com/euroargodev/OSnet-GulfStream&branch=binder

Launch Binder with Jupyterlab at your root repo level:
https://mybinder.org/v2/gh/euroargodev/binder-sandbox/main?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Feuroargodev%252FOSnet-GulfStream%26urlpath%3Dlab%252Ftree%252FOSnet-GulfStream%252F%26branch%3Dbinder

https://mybinder.org/v2/gh/euroargodev/binder-sandbox/main?urlpath=git-pull?repo=https://github.com/euroargodev/OSnet-GulfStream&urlpath=lab/tree/OSnet-GulfStream/docs/&branch=binder



Launch Binder with Jupyterlab and open a specific notebook:

https://mybinder.org/v2/gh/euroargodev/binder-sandbox/main?urlpath=git-pull%3Frepo%3Dhttps%253A%252F%252Fgithub.com%252Feuroargodev%252FOSnet-GulfStream%26urlpath%3Dlab%252Ftree%252FOSnet-GulfStream%252Fdocs%252Fdemo-predictions.ipynb%26branch%3Dbinder




https://mybinder.org/v2/gh/euroargodev/binder-sandbox/main?urlpath=git-pull?repo=https://github.com/euroargodev/OSnet-GulfStream&urlpath=lab/tree/OSnet-GulfStream/docs/demo-predictions.ipynb&branch=binder

Open this repo:
[![badge](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Binder&message=GCE+us-central1&color=blue)](https://binder.pangeo.io/v2/gh/euroargodev/binder-sandbox/master?urlpath=lab)

Open another repo:
[![Binder](https://img.shields.io/static/v1.svg?logo=Jupyter&label=Binder&message=Open+with+Pangeo&color=blue)](https://binder.pangeo.io/v2/gh/euroargodev/binder-sandbox/master?urlpath=git-pull?repo=https://github.com/euroargodev/argopy)

