# AminStoneKonig_avoidance-dopamine_2026
Code and data to accompany https://www.biorxiv.org/content/10.1101/2025.07.07.663268v1

Other previously published code used in the manuscript can be found at https://github.com/bidaye-lab/Sapkal_et_al_2024 and https://github.com/DavideR2020/NOSA.

Code is organized into folders by figure, with the exception of the envs folder which contains conda environment files for running the code in the notebooks. See the readme in the envs folder for installation instructions and for which environment to use with which files.

Note that code for figure S10 in in the fig5_figS10-modeling folder, and the code for Fig. 1j, Extended Data Fig. 1b,e, and Supplemental Data Synapse Topology are in the synpatic-sites notebooks in the fig2-connectome folder along with the code for Fig. 2a-e.

### System Requirements
All code has been tested on a 2021 Macbook Pro M1 Max running Tahoe 26.3.
Software dependencies are specified in the conda environment files in the envs folder, and there is no non-standard hardware required.

### Installation instructions

#### Prerequisites
Conda or Miniconda

#### Clone the repository
`git clone https://github.com/syncrostone/AminStoneKonig_avoidance-dopamine_2026.git`
`cd AminStoneKonig_avoidance-dopamine_2026`

#### Create and activate the appropriate conda environment

`cd envs`

Install the environment using conda with the command `conda env create -f ENV_NAME.yml`, where `ENV_NAME.yml` is the name of the environment file you want to install. For example, to install the environment needed to run the FAFB synaptic sites notebooks, use `conda env create -f ENV_FAFB.yml`. Then, select the correct environment for the kernel of the Jupyter notebook, e.g. 'FAFB' to run the FAFB synaptic sites notebok. See the table below for more information on which environment is needed for which notebook.

| .yml file | Environment | Notes |
| --- | --- | --- |
| ENV_FAFB.yml | FAFB | Needed to run the `fig2-connectome/synapticSites-FAFB.ipynb` notebook, which contains code to create renderings of the MDNs in the brain and all their pre- and postsynaptic sites (Fig. 1j, 2a; Extended Data Fig. 1b; Supplemental Data Synapse Topology) and of the Bolt neurons (Extended Data Fig. 1e) It contains the flywire python client, which is used to access the FAFB connectome data. |
| ENV_FANC.yml | FANC | Needed to run the `fig2-connectome/synapticSites-FANC.ipynb` notebook, which contains code to display LAL-MDN synapses (Fig. 2e; Supplemental Data Synapse Topology) and MBON-LAL synapses (Supplemental Data Synapse Topology). It contains the FANC python client, which is used to access the FANC connectome data. |
| ENV_stone.yml | model-and-connectome | Needed to run the `fig2-connectome/connectome_analysis.ipynb` notebook and the notebooks in `fig5_S10-modeling.scripts`. |
| ENV_barnstedt.yml | stats_plotting | Needed to run all other notebooks.



### Demo


### Usage









