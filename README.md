

[![Build Status](https://dev.azure.com/responsibleai/interpret-extensions/_apis/build/status/microsoft.interpret-community?branchName=master)](https://dev.azure.com/responsibleai/interpret-extensions/_build/latest?definitionId=5&branchName=master)
![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)
![versions](https://img.shields.io/badge/python-2.7%20%7C%203.6-blue)

Interpret Community Extensions SDK
=============================================================


The Interpret Community Extensions builds on [InterpretML](https://github.com/Microsoft/interpret), an open source python package from Microsoft Research for training interpretable models and explaining blackbox systems, by adding additional extensions from the community to interpret blackbox ML models.

This repository contains examples and best practices to use tools to assist in interpretability.

# Contents
(urls will be added once this is solidified)
- Try our notebooks
    - Launch them on Azure
- Getting Started 
- Models
- Contributing
- Code of Conduct
- Build Status
- Additional Info

# Try our notebooks
[![Azure Notebooks](https://notebooks.azure.com/launch.png)](https://notebooks.azure.com/import/gh/microsoft/interpret-community)

## Getting Started

# bz todo: make getting started a separate md page. Validate steps in clean env.

To setup on your local machine:

1. Install Anaconda with Python >= 3.6. [Miniconda](https://conda.io/miniconda.html) is a quick way to get started.

2. Clone the repository 
```
git clone https://github.com/Microsoft/Recommenders
```

3. Create conda environment
```
conda create -n interp python=3.6 anaconda

```
4. Activate conda environment
```
conda activate interp
or
activate interp
```

5. Install Python module, package and necessary distributions

   from the root folder:
```
python/pip install -e . 
```
6. Install additional packages for tests and more
```
pip install -r requirements.txt
```
7. Install scikit-learn
```
pip install sklearn
```
8. Set up and run Jupyter Notebook
```
activate interp
conda install nb_conda
pip install interpret
pip install jupyter
jupyter notebook
```
<!---{% from interpret.ext.blackbox import TabularExplainer %}
--->

# Models

# bz this section requires rewording
* The API supports both dense (numpy or pandas) and sparse (scipy) datasets
(verify?)
* For more advanced users, individual explainers can be used
 (details?)
* The TabularExplainer provides local and global feature importances (s?)  
    *  The best explainer is automatically chosen for the user based on the model
        - (how to define best)
* Local feature importances are for each evaluation row
* Global feature importances summarize the most importance features at the model-level
 * The KernelExplainer and MimicExplainer are for BlackBox models
 * The MimicExplainer is faster but less accurate than the KernelExplainer
 * The TreeExplainer is for tree-based models
 * The DeepExplainer is for DNN tensorflow or pytorch models
shap and lime have docs
others ?
global surrogate is 
# Contributing

# bz is CLA required when we go public?

This project welcomes contributions and suggestions.  Most contributions require you to agree to a
Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.

When you submit a pull request, a CLA bot will automatically determine whether you need to provide
a CLA and decorate the PR appropriately (e.g., status check, comment). Simply follow the instructions
provided by the bot. You will only need to do this once across all repos using our CLA.

# Code of Conduct

This project has adopted the [Microsoft Open Source Code of Conduct](https://opensource.microsoft.com/codeofconduct/).
For more information see the [Code of Conduct FAQ](https://opensource.microsoft.com/codeofconduct/faq/) or
contact [opencode@microsoft.com](mailto:opencode@microsoft.com) with any additional questions or comments.

# Build Status
# bz add detailed build status
[![Build Status](https://dev.azure.com/responsibleai/interpret-extensions/_apis/build/status/microsoft.interpret-community?branchName=master)](https://dev.azure.com/responsibleai/interpret-extensions/_build/latest?definitionId=5&branchName=master)

# Additional Info
