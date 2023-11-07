# REVIEW about the conda commands for usage of an open source GitHub repo. like [RVT algorithm](https://github.com/uzh-rpg/RVT.git)

## conda installation problem
- "can't find conda command": `export PATH=/path/to/the/conda/bin/:$PATH`; `source .bashrc`

## conda env 
- create env: `conda create -n <env-name> -y python=3.9 pip`
- delete env: `conda env remove -n <env-name>`
- activate env: `conda activate <env-name>`
- deactivate env: `conda deactivate`
- check all the created envs: `conda env list`
- conda依赖项的安装位置取决于conda（mambaforge/anaconda）等的安装位置
- `conda clean -a` 清除残留的数据文件
- `cd $CONDA_PREFIX` 快速进入当前conda环境所在文件夹

## conda dependencies
- check dependencies: `conda list`
- `conda config --set channel_priority flexible` 设定配置选项，允许按顺序从不同渠道获取conda包
- install dependencies: `conda install -y <pkg-name> -c pytorch -c nvidia -c conda-forge`
  - check the installation of dependencies in the .../env/<env-name>/lib/python3.9/site_packages folder
- 

## 深度学习相关

- `conda install -c "nvidia/label/cuda-11.8.0" cuda_toolkit 在[conda官网](https://anaconda.org/nvidia/cuda)下载cuda toolkit
- 
