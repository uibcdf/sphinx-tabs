# Build and Upload (`sphinx-tabs`)

## Prerequisites

```bash
conda install -c conda-forge conda-build anaconda-client
```

## Build package

Run from repository root:

```bash
conda build devtools/conda-build
```

Get the built package path:

```bash
conda build devtools/conda-build --output
```

## Upload to `uibcdf`

```bash
anaconda login
anaconda upload --user uibcdf <PACKAGE_PATH> --label main
anaconda logout
```

## Install from channel

```bash
conda install -c uibcdf sphinx-tabs
```
