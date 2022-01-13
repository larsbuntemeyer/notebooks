# Notebooks for prototyping

[![nbviewer](https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg)](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/tree/main/)


These notebooks contain some prototype code for working with large CMIP or CORDEX datasets. Most notebooks are not documented 
very well but are used only to try out some coding concepts. Most notebooks require data access to the 
[DKRZ data pool](https://www.dkrz.de/up/de-services/de-data-management/de-cmip-data-pool) using their intake catalogs. However, in principle
you should also be able to run CMIP6 notebooks if you switch to the [PANGEO datastore url](https://github.com/pangeo-data/pangeo-datastore).

* [`CMIP6-global-warming.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/CMIP6-global-warming.ipynb?flush_cache=true): data access, processing and plotting of CMIP6 data at DKRZ using `intake-esm` with `xarray` and `dask`.
* [`CMIP6-access-dkrz.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/CMIP6-access-dkrz.ipynb?flush_cache=true): data access and processing of CMIP6 data at DKRZ using `intake-esm` with `xarray` and `dask`.
* [`esgf.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/esgf.ipynb?flush_cache=true): access of cordex and cmip data from the ESGF via opendap protocol.
* [`shapefiles.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/shapefiles.ipynb?flush_cache=true): masking of cordex data by countries based on shapefiles.
* [`climdex-catalog.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/climdex-catalog.ipynb?flush_cache=true): plot climate indices from CMIP5 models at the DKRZ data pool.
* [`xclim-test.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/xclim-test.ipynb?flush_cache=true): compute CMIP6 climate indicators using [xclim](https://github.com/Ouranosinc/xclim) and dask.


## Requirements

The most important packages that will make your work with heavy cmip datasets easier are:

  - python=3
  - ipykernel
  - tqdm
  - pandas
  - matplotlib
  - xarray
  - dask
  - intake-esm
  - seaborn
  - fsspec
  - dask-jobqueue
  - ipywidgets
  - jupyter
  - cartopy
  - geoviews

You can use the `environment.yaml` file to easily install all dependencies, e.g.
```
conda env create -f environment.yaml
```

## Server settings - DKRZ

Here are my recommended server settings for the [JupyterLab at DKRZ](https://jupyterhub.dkrz.de).

![Server Settings DKRZ](server-settings-dkrz.png "Server Settings DKRZ")

