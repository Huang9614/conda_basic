# REVIEW about the conda commands for usage of an open source GitHub repo. like [RVT algorithm](https://github.com/uzh-rpg/RVT.git)

## conda installation problem
- "can't find conda command": `export PATH=/path/to/the/conda/bin/:$PATH`; `source .bashrc`

## conda env 
- create env: `conda create -n <env-name> -y python=3.9 pip`
- delete env: `conda env remove <env-name>`
- activate env: `conda activate <env-name>`
- deactivate env: `conda deactivate`

## conda dependencies
- check dependencies: `conda list`
- install dependencies: `conda install -y <pkg-name> -c pytorch -c nvidia -c conda-forge'
  - check the installation of dependencies in the env/ folder
-

