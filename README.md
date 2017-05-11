# Interactive Visualization Using HTML

by Chengping Chai, Charles J. Ammon, Monica Meceria and Robert B. Herrman

This package contains source code and data for two examples of plotting 3D seismic models using HTML. We use a dispersion model from Herrmann et al. (2013, http://www.eas.slu.edu/eqc/eqc_research/NATOMO/) and a 3D shear velocity model from Chai et al. ([GRL](http://onlinelibrary.wiley.com/doi/10.1002/2015GL063733/full), 2015, also at http://eqseis.geosc.psu.edu/~cchai/01research/01westernUS.html). The dispersion data and velocity model are included in the folders RAYLU and WUS-CAMH-2015, respectively. Our plots also use political boundaries and coastlines data that are prepared with GMT (http://gmt.soest.hawaii.edu/). The boundary data are provided for U.S. region in the  utility folder.

The python script plot_dispersion_as_html.py can be used to generate an interactive plot like http://eqseis.geosc.psu.edu/~cchai/WUS_dispersion_viewer.html. The python script plot_3D_model_as_html.py was used to generate a dynamic figure like http://eqseis.geosc.psu.edu/~cchai/WUS_model_viewer.html. The utility.py contains some Python functions used by the above two scripts.

## Install Required Package

The following python packages are required to generate interactive plots using our codes.

* numpy (version 1.10.4 and above)
* scipy (version 0.17.0 and above)
* bokeh (version 0.12.0 and above)

Installation through Anaconda (or Miniconda) is highly recommended. You can find instructions on how to install Anaconda at https://docs.continuum.io/anaconda/install.

Once you have Anaconda installed, the required packages can be installed using these commands in the terminal.

```bash
conda install numpy
conda install scipy
conda install bokeh
```

## Usage

To generate the HTML file for the dispersion model, type the following command in your terminal.

```bash
python plot_dispersion_as_html.py
```

The HTML file for the velocity model can be generated by the command below.

```bash
python plot_3D_model_as_html.py
```
