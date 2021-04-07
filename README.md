# WebConfTuto

Notebooks and material for the tutorial on networks analysis.

You can run them online by clicking on the binder button
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/epfl-lts2/GraphMining-TheWebConf2021/HEAD)

You can also run them locally from your computer, check the [Local installation](#local-installation) section

## Outline

The Tutorial will explore the world of (large) graphs using the following notebooks:
* `01_graph_from_edge_list.ipynb` is the introduction to building and handling a graph with Python, using `networkx`.
* `02_basic_graph_properties.ipynb` show the different standard methods and tools to get information about the graph structure (graph diameter, connectivity, degree distribution...)
* `03_graph_exploration_and_sampling.ipynb` presents the algorithms for large graph exploration and graph sampling,
* `04_ML_on_graphs.ipynb` proposes to experiment with unsupervised and semi-supervised machine learning on graphs,
* `05_Reddit_Pushshift_API.ipynb` show in practice how to explore the Reddit social network through the Reddit Pushshift API.

![Reddit neighbors](figures/redditneighbors.png "Reddit neighbors")

## Local installation

If you prefer using the notebooks locally instead of running them on binder, you need to set
up a number of tools.

For a local installation, you will need [git], [Python], and packages from the [Python scientific stack][scipy].
If you don't know how to install those on your platform, we recommend to install [Miniconda] or [Anaconda], a distribution of the [conda] package and environment manager.
Follow the below instructions to install it and create an environment for the course.

1. Download the Python 3.x installer for Windows, macOS, or Linux from <https://conda.io/miniconda.html> and install with default settings.
   Skip this step if you have conda already installed (from [Miniconda] or [Anaconda]).
   * Windows: double-click on `Miniconda3-latest-Windows-x86_64.exe`.
   * macOS: double-click on `Miniconda3-latest-MacOSX-x86_64.pkg` or run `bash Miniconda3-latest-MacOSX-x86_64.sh` in a terminal.
   * Linux: run `bash Miniconda3-latest-Linux-x86_64.sh` in a terminal or use your package manager.
1. Open a terminal.
   Windows: open the Anaconda Prompt from the Start menu.
1. Install git with `conda install git`.
1. Navigate to the folder where you want to store the course material with `cd path/to/folder`.
1. Download this repository with `git clone https://github.com/epfl-lts2/GraphMining-TheWebConf2021`.
1. Enter the repository with `cd GraphMining-TheWebConf2021`.
1. Create an environment with the packages required for the course with `conda env create -f environment_local.yml`.

Every time you want to work, do the following:

1. Open a terminal.
   Windows: open the Anaconda Prompt from the Start menu.
1. Activate the environment with `conda activate graphmining-twc21-local`.
1. Navigate to the folder where you stored the course material with `cd path/to/folder/GraphMining-TheWebConf2021`.
1. Start Jupyter with `jupyter lab`.
   The command should open a new tab in your web browser.
1. Edit and run the notebooks from your browser.
1. Once done, you can run `conda deactivate` to leave the `graphmining-twc21-local` environment.

[git]: https://git-scm.com
[python]: https://www.python.org
[scipy]: https://www.scipy.org
[anaconda]: https://www.anaconda.com/download
[miniconda]: https://conda.io/miniconda.html
[conda]: https://conda.io
[conda-forge]: https://conda-forge.org



