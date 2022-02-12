# geohoods-to

This document details steps to reproducing the `geohoods-to` dataset.

## Install

1. Install [Anaconda 3](https://www.anaconda.com/)
2. Run ``bin/install`` to create a ``conda`` environment
3. Activate the ``conda`` environment (under ``tmp/``)

In Windows:

```
bin\install
bin\activate
```

In Linux/Mac OS:

```
source bin/install.sh
source bin/activate.sh
```

## Usage

To reproduce the dataset:

1. Run the jupyter notebook interface with ``bin/notebook``
2. Open [src/download.ipynb](src/download.ipynb) and run all cells (this downloads all the raw data)
3. Open [src/preprocess.ipynb](src/preprocess.ipynb) and run all cells (this cleans the raw data)
4. Open [src/run.ipynb](src/preprocess.ipynb) and run all cells (this produces the final datasets)
5. A folder with the final data should be processed under the ``tmp/dist`` folder

In Windows:

```
bin\notebook
```

In Linux/Mac OS:

```
source bin/notebook.sh
```

## Hardware

Mac Mini (M1, 2020)
Apple M1 CPU 8-Core
16 GB RAM
250GB SSD

Approximate running times for latest release:

1. [src/download.ipynb](src/download.ipynb): 1 min
2. [src/preprocess.ipynb](src/preprocess.ipynb): 3 min
3. [src/run.ipynb](src/preprocess.ipynb): 36 min