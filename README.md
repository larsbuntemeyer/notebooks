# notebooks for prototyping

These notebooks contain some prototype code for working with large CMIP or CORDEX datasets. Most notebooks are not documented 
very well but are used only to try out some coding concepts.

* [`CMIP6-access-dkrz.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/CMIP6-access-dkrz.ipynb): data access and processing of CMIP6 data at DKRZ using `intake-esm` with `xarray` and `dask`.
* [`esgf.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/esgf.ipynb): access of cordex and cmip data from the ESGF via opendap protocol.
* [`shapefiles.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/shapefiles.ipynb): masking of cordex data by countries based on shapefiles.
* [`climdex-catalog.ipynb`](https://nbviewer.jupyter.org/github/larsbuntemeyer/notebooks/blob/main/climdex-catalog.ipynb): plot climate indices from CMIP5 models at the DKRZ data pool.

## requirements

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
  - holoviews
  - hvplot
  - cartopy
  - geoviews

You can use the `environment.yaml` file to easily install all dependencies, e.g.
```
conda env create -f environment.yaml
```
