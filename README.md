[English](./README.md) / [Spanish](./README_es.md) / [Korean](./README_ko.md) / [Chinese](./README_zh.md) / [Bengali](./README_bn.md) / [Indonesian](./README_id.md) / [Italian](./README_it.md) / [Portuguese](./README_pt.md) / [Vietnamese](./README_vn.md) / [Japanese](./README_ja.md)

# How to run these notebooks
- Open notebook folder on Visual Studio Code.
- Open the terminal of Visual Studio Code. The path should point to the root folder.
- Type `jupyter notebook` or `python -m jupyter notebook` and Enter. The notebook should open on a new browser tab. The reason for `python -m` is if you don't have pip on environment variables.

# Register python scripts on Windows Environment Variables
- If you don't want to keep typing `python -m` on every run and are using Windows platform, you can follow this instructions.
- To test if you have already registered the python scripts on environment variables, open a new command prompt and type `pip --version`. If the command returns correct version, you have already registered the scripts to environment variables. Otherwise, continue.
- First, find the location of your python scripts. Type `where python` on command prompt. It should return python location, such as `C:\Users\username\miniforge3\python.exe`.
- The location you need is the "Scripts" folder on the sibling location. For example, this case would be `C:\Users\username\miniforge3\Scripts`.
- Now, go to Windows Search and find `Edit the system environment variables`.
- Click Environment Variables on bottom-right.
- Choose either "user variables" or "system variables". The difference between the two is "user variables" will only change the setting for your user account, while "system variables" change will be applied to all user accounts on the computer.
- Find variable "Path" and edit it.
- Add the scripts location from earlier, i.e. `C:\Users\username\miniforge3\Scripts`
- Confirm all changes. To test, open a new command prompt and type `pip --version`.

# Error graphviz, gv command
- If graphviz, gv command doesn't work with error: `failed to execute Path('dot'), make sure the Graphviz executables are on your systems' PATH`, run the instruction from https://github.com/RedaOps/ann-visualizer/issues/12.
- Install graphviz from https://graphviz.org/download/ if you haven't already and you have error when running gv command.
- You may need to restart your computer for the changes to take effec.

# The fastai book

These notebooks cover an introduction to deep learning, [fastai](https://docs.fast.ai/), and [PyTorch](https://pytorch.org/). fastai is a layered API for deep learning; for more information, see [the fastai paper](https://www.mdpi.com/2078-2489/11/2/108). Everything in this repo is copyright Jeremy Howard and Sylvain Gugger, 2020 onwards. A selection of chapters is available to [read online here](https://fastai.github.io/fastbook2e/).

The notebooks in this repo are used for [a MOOC](https://course.fast.ai) and form the basis of [this book](https://www.amazon.com/Deep-Learning-Coders-fastai-PyTorch/dp/1492045527), which is currently available for purchase. It does not have the same GPL restrictions that are on this repository.

The code in the notebooks and python `.py` files is covered by the GPL v3 license; see the LICENSE file for details. The remainder (including all markdown cells in the notebooks and other prose) is not licensed for any redistribution or change of format or medium, other than making copies of the notebooks or forking this repo for your own private use. No commercial or broadcast use is allowed. We are making these materials freely available to help you learn deep learning, so please respect our copyright and these restrictions.

If you see someone hosting a copy of these materials somewhere else, please let them know that their actions are not allowed and may lead to legal action. Moreover, they would be hurting the community because we're not likely to release additional materials in this way if people ignore our copyright.

## Colab

Instead of cloning this repo and opening it on your machine, you can read and work with the notebooks using [Google Colab](https://research.google.com/colaboratory/). This is the recommended approach for folks who are just getting started -- there's no need to set up a Python development environment on your own machine, since you can just work directly in your web-browser.

You can open any chapter of the book in Colab by clicking on one of these links: [Introduction to Jupyter](https://colab.research.google.com/github/fastai/fastbook/blob/master/app_jupyter.ipynb) | [Chapter 1, Intro](https://colab.research.google.com/github/fastai/fastbook/blob/master/01_intro.ipynb) | [Chapter 2, Production](https://colab.research.google.com/github/fastai/fastbook/blob/master/02_production.ipynb) | [Chapter 3, Ethics](https://colab.research.google.com/github/fastai/fastbook/blob/master/03_ethics.ipynb) | [Chapter 4, MNIST Basics](https://colab.research.google.com/github/fastai/fastbook/blob/master/04_mnist_basics.ipynb) | [Chapter 5, Pet Breeds](https://colab.research.google.com/github/fastai/fastbook/blob/master/05_pet_breeds.ipynb) | [Chapter 6, Multi-Category](https://colab.research.google.com/github/fastai/fastbook/blob/master/06_multicat.ipynb) | [Chapter 7, Sizing and TTA](https://colab.research.google.com/github/fastai/fastbook/blob/master/07_sizing_and_tta.ipynb) | [Chapter 8, Collab](https://colab.research.google.com/github/fastai/fastbook/blob/master/08_collab.ipynb) | [Chapter 9, Tabular](https://colab.research.google.com/github/fastai/fastbook/blob/master/09_tabular.ipynb) | [Chapter 10, NLP](https://colab.research.google.com/github/fastai/fastbook/blob/master/10_nlp.ipynb) | [Chapter 11, Mid-Level API](https://colab.research.google.com/github/fastai/fastbook/blob/master/11_midlevel_data.ipynb) | [Chapter 12, NLP Deep-Dive](https://colab.research.google.com/github/fastai/fastbook/blob/master/12_nlp_dive.ipynb) | [Chapter 13, Convolutions](https://colab.research.google.com/github/fastai/fastbook/blob/master/13_convolutions.ipynb) | [Chapter 14, Resnet](https://colab.research.google.com/github/fastai/fastbook/blob/master/14_resnet.ipynb) | [Chapter 15, Arch Details](https://colab.research.google.com/github/fastai/fastbook/blob/master/15_arch_details.ipynb) | [Chapter 16, Optimizers and Callbacks](https://colab.research.google.com/github/fastai/fastbook/blob/master/16_accel_sgd.ipynb) | [Chapter 17, Foundations](https://colab.research.google.com/github/fastai/fastbook/blob/master/17_foundations.ipynb) | [Chapter 18, GradCAM](https://colab.research.google.com/github/fastai/fastbook/blob/master/18_CAM.ipynb) | [Chapter 19, Learner](https://colab.research.google.com/github/fastai/fastbook/blob/master/19_learner.ipynb) | [Chapter 20, conclusion](https://colab.research.google.com/github/fastai/fastbook/blob/master/20_conclusion.ipynb)


## Contributions

If you make any pull requests to this repo, then you are assigning copyright of that work to Jeremy Howard and Sylvain Gugger. (Additionally, if you are making small edits to spelling or text, please specify the name of the file and a very brief description of what you're fixing. It's difficult for reviewers to know which corrections have already been made. Thank you.)

## Citations

If you wish to cite the book, you may use the following:

```
@book{howard2020deep,
title={Deep Learning for Coders with Fastai and Pytorch: AI Applications Without a PhD},
author={Howard, J. and Gugger, S.},
isbn={9781492045526},
url={https://books.google.no/books?id=xd6LxgEACAAJ},
year={2020},
publisher={O'Reilly Media, Incorporated}
}
```

