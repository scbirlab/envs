# Conda environments

Conda environment definition files for making environments that are useful for various analysis tasks.

Most have been validated to work on NEMO.

## Usage

The up-to-date version of an environment called `<env-name>` can be installed with the basic command:

```{bash}
conda env create -f https://raw.githubusercontent.com/scbirlab/envs/main/<env-name>.yml --force
```

This can take several minutes to complete. If mamba is installed on your system (as is the case on NEMO), 
substituting `conda` for `mamba` may be faster. 

For example, to install the `basic` environment:

```{bash}
mamba env create -f https://raw.githubusercontent.com/scbirlab/envs/main/basic.yml
```

## Environments

### basic

This is a general-purpose environment for data analysis, machine learning, and chemistry.
It provides Jupyter Notebooks, [`rdkit`](https://github.com/rdkit/rdkit), and GPU versions 
of [`tensorflow`](https://github.com/tensorflow/tensorflow), and [`jax`](https://github.com/google/jax) 
which are compatible with NEMO.

```{bash}
mamba env create -f https://raw.githubusercontent.com/scbirlab/envs/main/basic.yml --force
```

### chemprop

Installs Jupyter Notebooks and GPU version of [`pytorch`](https://github.com/pytorch/pytorch) and 
[`chemprop`](https://github.com/chemprop/chemprop) compatible with NEMO.

```{bash}
mamba env create -f https://raw.githubusercontent.com/scbirlab/envs/main/chemprop.yml --force
```

### chemprop

Installs tools for developing Python packages and other software.

```{bash}
mamba env create -f https://raw.githubusercontent.com/scbirlab/envs/main/dev.yml --force
```

### oligo-design

Installs [`monte-barcode`](https://github.com/scbirlab/monte-barcode) and [`ogilo-array`](https://github.com/scbirlab/ogilo) 
for designing barcoded oligo pools.

```{bash}
mamba env create -f https://raw.githubusercontent.com/scbirlab/envs/main/oligo-design.yml --force
```

## Issues, problems, suggestions

Add to the [issue tracker](https://www.github.com/scbirlab/envs/issues).

## Further help

Here are the help pages of the software installed in these environments.

- [`rdkit`](https://rdkit.org/docs/RDKit_Book.html)
- [`tensorflow`](https://www.tensorflow.org/)
- [`jax`](https://jax.readthedocs.io/en/latest/#) 
- [`pytorch`](https://pytorch.org/)
- [`chemprop`](https://chemprop.readthedocs.io/en/latest/)
- [`monte-barcode`](https://monte-barcode.readthedocs.io/en/latest/)
- [`ogilo-array`](https://ogilo.readthedocs.io/en/latest/)