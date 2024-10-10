[![](https://img.shields.io/badge/ExploreData-DatasetteLite-blue)](https://lite.datasette.io/?metadata=https://raw.githubusercontent.com/swinnoproject/datasette-lite/refs/heads/main/metadata.yml&url=https://zenodo.org/api/records/13893763/files/SWINNO.UDIT.sqlite3/content
)

# SWINNO and Datasette(Lite)

This repository hosts a metadata file that is
intended to be used with [Datasette](https://github.com/simonw/datasette) or [DatasetteLite](https://github.com/simonw/datasette-lite) to enable explorations of the [SWINNO data](https://doi.org/10.5281/zenodo.13893763)

## DatasetteLite

DatasetteLite is a lightweight version of Datasette
that runs in your browser. It does not require you
to download or install anything -- but it can take
a few minutes before everything is set up.

## Datasette

Datasette can also be installed and run locally thorugh `brew` or it can be installed as a python package through pip.

On a mac with homebrew installed you can:

```brew install datasette```

On other devices you first need to install [Python](https://www.python.org/) and then you can install datasette through the Python package infrastructure `pip`:

```python -m pip install datasette```

Or through the `pipx`:

```pipx install datasette```

For more details on installation and basic usage see the datasette code repository: https://github.com/simonw/datasette

### Download the data

The latest version of the SQLite3 file can always be downloaded from [zenodo](https://doi.org/10.5281/zenodo.13893763).

### metadata.yml

The `metadata.yml` file contains some descriptive information about the project as well as some standardised queries to get you started with exploring the data. In order to load it with your database

To load the metadata file you simply have to run:

```datasette /path/to/database.file --metadata /path/to/metadata.yml```
