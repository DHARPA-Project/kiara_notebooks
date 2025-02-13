# kiara_notebooks
Jupyter Notebooks for kiara

This repository contains Jupyter Notebooks using <i>kiara</i> that can be used as an introductory guide to <i>kiara</i> and it's language in Jupyter. You can either clone this repository, or download the notebooks individually - just make sure to also download the relevant data for each notebook as well!

Before using any notebooks, <i>kiara</i> needs to be installed via the CLI as follows.

First install conda and / or miniconda. Installation instructions for miniconda can be found [here](https://docs.anaconda.com/miniconda/). Make sure to double check that you are installing the right version for your device, including which system your device is currently running on. 

Launch your CLI shell.

Create an environment to install <i>kiara</i> into. Future documentation may want to include or point to more information on the role of environments in coding (I think this would be useful for novice coders or other users unfamiliar with managing and testing code), e.g. https://docs.anaconda.com/working-with-conda/environments/

```
conda create -n kiara_testing
```

Feel free to replace `kiara_testing` with any chosen environment name. At this stage, I'm successfully running <i>kiara</i> on Python 3.13.0.

Next activate the conda environment.

```
conda activate kiara_testing
```

Now we want to start installing packages. Note that conda can be used to install any standard python packages, but pip has to be used for <i>kiara</i>.

```
pip install kiara
```

The first installation of <i>kiara</i> may take a little while, but not too long. After this, we want to include the relevant <i>kiara</i> plugins, as follows:

```
pip install kiara_plugin.core_types kiara_plugin.onboarding kiara_plugin.tabular
```

At time of writing, the versions installed are as follows:

```
kiara                     0.5.13
kiara_plugin.core_types   0.5.2
kiara_plugin.onboarding   0.5.2
kiara_plugin.tabular      0.5.6
```

To check which version of <i>kiara</i> or any of its plugins are installed at any point, type ```pip list | grep kiara ``` into the CLI.

Depending on which notebooks you wish to run, you may also need to install the plugins for topic modelling and network analysis.
