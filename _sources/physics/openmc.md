# OpenMC

## Install

```bash
conda config --add channels conda-forge

conda create -y -n openmc-env
conda activate openmc-env

conda install -y mamba

mamba search openmc
mamba install openmc

sudo conda install -y -n openmc-env ipykernel

hdf5_data_path=~/nuclear_data/hdf5/jeff-3.3-hdf5
mkdir -p $hdf5_data_path
curl -L -o jeff33.tar.xz https://anl.box.com/shared/static/4jwkvrr9pxlruuihcrgti75zde6g7bum.xz
tar -xvf jeff33.tar.xz -C $hdf5_data_path
rm jeff33.tar.xz

chain_data_path=~/nuclear_data/hdf5/simplified_chain
mkdir -p $chain_data_path
curl -L -o chain_casl_pwr.xml https://anl.box.com/shared/static/nyezmyuofd4eqt6wzd626lqth7wvpprr.xml
mv chain_casl_pwr.xml $chain_data_path
```