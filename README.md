# Conda environments

Conda environment definition files for making environments that are useful for various analysis tasks.

Most have been validated to work on NEMO.

## Usage

The up-to-date version of an environment called `<env-name>` can be installed with the basic command:

```{bash}
conda env create --force -f https://github.com/scbirlab/envs/raw/main/<env-name>.yml
```

This can take several minutes to complete. If mamba is installed on your system (as is the case on NEMO), 
substituting `conda` for `mamba` may be faster. 

For example, to install the `basic` environment:

```{bash}
mamba env create --force -f https://github.com/scbirlab/envs/raw/main/basic.yml
```

Other versions can be installed by replacing `main` with the version name, for example `v0.0.1`:

```{bash}
mamba env create --force -f https://github.com/scbirlab/envs/raw/v0.0.1/basic.yml 
```

## Environments

### basic

This is a general-purpose environment for data analysis, machine learning, and chemistry.
It provides Jupyter Notebooks, [`rdkit`](https://github.com/rdkit/rdkit), and GPU versions 
of [`tensorflow`](https://github.com/tensorflow/tensorflow), and [`jax`](https://github.com/google/jax) 
which are compatible with NEMO.

```{bash}
mamba env create --force -f https://github.com/scbirlab/envs/raw/main/basic.yml
```

### chemprop

Installs Jupyter Notebooks and GPU version of [`pytorch`](https://github.com/pytorch/pytorch) and 
[`chemprop`](https://github.com/chemprop/chemprop) compatible with NEMO.

```{bash}
mamba env create --force -f https://github.com/scbirlab/envs/raw/main/chemprop.yml
```

### chem-llm

This is an environment for large language modelling for chemistry.
It provides Jupyter Notebooks, [`rdkit`](https://github.com/rdkit/rdkit), and GPU versions 
of [`tensorflow`](https://github.com/tensorflow/tensorflow), [`flax`](https://github.com/google/flax),
[`pytorch`](https://github.com/pytorch/pytorch), and [`🤗 transformers`](https://github.com/huggingface/transformers)
which are compatible with NEMO.

```{bash}
mamba env create --force -f https://github.com/scbirlab/envs/raw/main/chem-llm.yml
```

### dev

Installs tools for developing Python packages and other software.

```{bash}
mamba env create --force -f https://github.com/scbirlab/envs/raw/main/dev.yml
```

### hts-tools

Installs [`hts-tools`](https://github.com/scbirlab/hts-tools) for analyzing platereader data.

```{bash}
mamba env create --force -f https://github.com/scbirlab/envs/raw/main/hts.yml
```

### oligo-design

Installs [`monte-barcode`](https://github.com/scbirlab/monte-barcode) and [`ogilo`](https://github.com/scbirlab/ogilo) 
for designing barcoded oligo pools.

```{bash}
mamba env create --force -f https://github.com/scbirlab/envs/raw/main/oligo-design.yml
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
- [`🤗 transformers`](https://huggingface.co/docs/transformers)
- [`hts-tools`](https://hts-tools.readthedocs.io/en/latest/)
- [`monte-barcode`](https://monte-barcode.readthedocs.io/en/latest/)
- [`ogilo`](https://ogilo.readthedocs.io/en/latest/)