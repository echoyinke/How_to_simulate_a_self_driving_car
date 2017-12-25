# 如何模拟一个无人驾驶汽车

This is the code for "How to Simulate a Self-Driving Car" by Siraj Raval on Youtube

## 概述

这里是[该视频的相关代码](https://youtu.be/EaY5QiZwSP4)。 我们使用Udacity's [无人驾驶模拟器](https://github.com/udacity/self-driving-car-sim)来产生数据以及训练模型。

## 依赖

你可以通过运行下面的命令来安装依赖。

你需要 先安装[anaconda](https://www.continuum.io/downloads) or [miniconda](https://conda.io/miniconda.html) 以便来进行环境设置。

```python
# Use TensorFlow without GPU
conda env create -f environments.yml 

# Use TensorFlow with GPU
conda env create -f environment-gpu.yml
```

或者你也可以用`pip install`手动的安装需要的库 (参看 environemnt*.yml 文件的内容) 。

## 使用方法

### 运行事先训练好的模型

打开 [优达学城的无人驾驶模拟器](https://github.com/udacity/self-driving-car-sim), 选择场景和自动驾驶模式，然后运行下面的命令：

```python
python drive.py model.h5
```

### 训练模型

你需要一个文件夹来存储训练时候产生的图片.

```python
python model.py
```

这会产生一个文件 `model-<epoch>.h5` 每个时间段（epoch）都会产生一个文件 .  比如，第一个时间段产生的就叫做 `model-000.h5`.

## Credits

代码来自 [naokishibuya](https://github.com/naokishibuya). 这里仅仅又包了一层来帮助大家着手与理解.



