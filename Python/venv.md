# 建立venv
### step
1. mkdir xx
2. cd xx
3. python -m venv xx_env

## 啟動venv
### step
1. cd xx
2. source cc_env/bin/actuvate


# 其他指令
可印出當前虛擬環境有什麼package
pip3 list




# 用conda建立及管理python虛擬環境
#### Step 1:安裝及更新conda 
1. conda update conda
2. 
#### Step 2:建立虛擬環境
1. conda create --name myenv python=3.5

看目前系統已經安裝幾個虛擬環境
conda env list

####  Step 3:啟動虛擬環境
1. activate myenv
2. source activate myenv (macOS or LINUX)

- install package
conda install numpy pandas os time 

#### Step 4:離開虛擬環境
1. deactivate
2. source deactivate (macOS or LINUX)

#### Step 5:刪除虛擬環境或package
1. conda remove --name myenv numpy
2. conda env remove --name myenv


