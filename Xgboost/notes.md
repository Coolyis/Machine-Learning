## Xgboost

#### 1.1 安装和导包

下载网址

> **xgboost documents：**https://xgboost.readthedocs.io/en/latest/index.html

首先确保正确安装Xgboost, 安装代码如下：

```python
# windows
pip install xgboost
pip install --upgrade xgboost

# mac
pip3 install xgboost
```

安装完成后，开始导入：

```python
import xgboost as xgb
```

#### 1.2 Xgboost介绍

现在，有两种方式来使用xgboost, 第一种方式是直接用xgboost自己的建模流程，第二种方式是使用sklearn中的API

1. 使用xgboost自己的建模流程 - 核心：DMtarix读取数据的类，以及用train()来训练这个数据的类
   与sklearn不同，需先试用字典来定义好参数集，再使用train()来将其作为参数进行训练
2. 使用sklearn中的API来进行建模

两种方式的建模流程类似，参数名称不同但用处一致，在xgboost本身的建模环境中运算速度（尤其是cross- validation）快，调参快捷
