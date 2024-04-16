Python Basics & Introductory Flopy example
-----------------------------------------------

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ebake310/GW_Model_GEOSC209.git/HEAD)

## Running the example
There are two ways to run the example:

1) [online via Binder](https://mybinder.org/v2/gh/aleaf/pleasant-lake-flopy-example/HEAD?labpath=worked_flopy_example.ipynb)
2) Locally on your computer, after creating a suitable python environment

### Running the example locally

1) Download and install the 64-bit [Anaconda python distribution](https://www.anaconda.com/distribution/) or [Miniconda](https://docs.conda.io/en/latest/miniconda.html)

  * Anaconda comes with a larger selection of popular data science and scientific packages, making it ideal for those who use python frequently for scientific computing.
  * Miniconda is a minimal installer with a much smaller footprint, making it ideal for those who only want to run this example.
  * **Make sure to install Anaconda or Miniconda to your username** (not at the system level). 

2) Create a [Conda environment](https://docs.conda.io/projects/conda/en/latest/user-guide/concepts/environments.html)

    Open an Anaconda Command Prompt on Windows or a terminal window on OSX and point it to the location of ``environment.yml`` and enter:

        conda env create -f environment.yml

    **Note:** if the above line executes too slowly, try installing [Mamba](https://mamba.readthedocs.io/en/latest/) and using that instead, i.e.

        mamba env create -f environment.yml

3) Activate the environment
    
    Open an Anaconda Command Prompt on Windows or a terminal window on OSX and enter:

        conda activate flopy_example

4) Run the Notebook

    Make sure that the command window with the conda environment activated is pointed at this folder, or any higher location in the file system. Then enter:

        jupyter notebook

    A new browser tab should pop up with the Jupyter file browser. Navigate to ``worked_flopy_example.ipynb`` and click on it. For more information on Jupyter Notebooks, refer to the documentation: https://jupyter.org.

    **Note:** Running the model through Flopy (as in the Notebook) requires specification of the MODFLOW executable. In the example, we assume that a MODFLOW 6 executable named ``"mf6"`` is visible in the system path at the location of this folder (see the ``exe_name`` argument in Notebook cell 5). Executables for MODFLOW 6 for linux, mac and windows are included in the ``bin/`` folder.
