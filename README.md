# Napari exercises

## Testing Napari viewer

Create the environment.
```
conda create -y -n napari-env -c conda-forge python=3.9
```

Activate it
```
conda activate napari-env
```

install napari
```
conda install -c conda-forge napari pyqt
```
or
```
pip install "napari[all]"
```

Run/open napari
```
napari
```

## Testing dev-bio napari plugin
Create the environment with napari and [dev-bio](https://github.com/haesleinhuepf/devbio-napari) set of plugins.
```
conda create --name dbn39 python=3.9 devbio-napari napari==0.4.18 pyqt -c conda-forge
```

Activate the environment using .
```
conda activate dbn39
```

Run napari assistant.
```
naparia
```

## Exporting rnviroment
```
conda env export > environment.yml
```

## Bonus: Jupyter Lab
```
conda install mamba -c conda-forge
mamba create --name julab python=3.9 jupyterlab -c conda-forge
conda activate julab
```
optional: Code Formatting Jupyter Notebooks with Black
```
mamba install -c conda-forge jupyterlab_code_formatter black isort
```
