# install conda
```
wget https://repo.anaconda.com/miniconda/Miniconda3-py39_4.9.2-Linux-x86_64.sh
chmod +x Miniconda3-py39_4.9.2-Linux-x86_64.sh
./Miniconda3-py39_4.9.2-Linux-x86_64.sh
source PATH_TO_MINICONDA/miniconda3/etc/profile.d/conda.sh
```

# create conda env and fill it up
```
conda config --add channels conda-forge 
conda create --name fink-nb python=3.7
conda activate fink-nb
git clone git@github.com:astrolabsoftware/fink-notebook-template.git
cd fink-notebook-template/
conda install numpy pandas matplotlib gatspy seaborn jupyter requests
pip install fink-science pyLIMA
```

# run jupyter
```jupyter notebook```

