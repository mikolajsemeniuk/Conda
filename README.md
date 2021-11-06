# Conda
```sh
# version
conda -V
conda --version
where python

dir C:\Users\{username}\miniconda3\envs

nvcc -V
nvcc --version

# update
conda update python
conda update conda

# show all environments, env with * is active
conda info --envs
conda env list

# show current active env
echo $CONDA_DEFAULT_ENV
conda info

# create new env
conda create -n ENV_NAME python=3.9
conda env create --file FILE # no need to name when created from .yaml
conda env create --name NAME --file FILE # from .yaml file

# activate/deactivate env
conda activate ENV_NAME
conda deactivate # change active env to `base`

# packages
conda install -n ENV_NAME PACKAGE_NAME # install latest package in active env
conda install scipy=0.15.0 # install pakcage with certain version  in active env
conda install scipy curl # multiple packages at once in active env
conda install scipy=0.15.0 curl=7.26.0 -n py34_env # install multiple packages with version in certain env
conda list -n ENV_NAME # list all installed packages in certain env
conda update -n ENV_NAME scipy # update package in certain env

# remove
conda env remove -n my # remove env
conda remove -n myenv scipy # remove package in certain env
conda remove scipy # remove package in active env

# exec python files
python myfile.py # REMEMBER TO USE CONDA PROMPT
```
