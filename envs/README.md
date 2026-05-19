This folder contains environment files for running the code in the notebooks.

Install the environment using conda with the command `conda env create -f ENV_NAME.yml`, where `ENV_NAME.yml` is the name of the environment file you want to install. For example, to install the environment needed to run the FAFB synaptic sites notebooks, use `conda env create -f ENV_FAFB.yml`. Then, select the FAFB environment for the kernel of the Jupyter notebook.See the table below for more information on which environment is needed for which notebook.

| .yml file | Environment | Notes |
| --- | --- | --- |
| ENV_FAFB.yml | FAFB | Needed to run the `fig2-connectome/synapticSites-FAFB.ipynb` notebook, which contains code to create renderings of the MDNs in the brain and all their pre- and postsynaptic sites (Fig. 1j, 2a; Extended Data Fig. 1b; Supplemental Data Synapse Topology) and of the Bolt neurons (Extended Data Fig. 1e) It contains the flywire python client, which is used to access the FAFB connectome data. |
| ENV_FANC.yml | FANC | Needed to run the `fig2-connectome/synapticSites-FANC.ipynb` notebook, which contains code to display LAL-MDN synapses (Fig. 2e; Supplemental Data Synapse Topology) and MBON-LAL synapses (Supplemental Data Synapse Topology). It contains the FANC python client, which is used to access the FANC connectome data. |
| ENV_stone.yml | model-and-connectome | Needed to run the `fig2-connectome/connectome_analysis.ipynb` notebook and the notebooks in `fig5_S10-modeling/scripts`. |
| ENV_barnstedt.yml | stats_plotting | Needed to run all other notebooks.
