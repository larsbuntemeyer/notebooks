# notebooks for prototyping

* `CMIP6-access-dkrz.ipynb`: data access and processing of CMIP6 data at DKRZ.
* `esgf.ipynb`: access of cordex and cmip data via opendap protocol.
* `shapefiles.ipynb`: masking cordex data by countries based on shapefiles.
* `climdex-catalog.ipynb`: plot climate indices from CMIP5 models.


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
