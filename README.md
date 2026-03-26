# 三角形旋转与变换

基于 Taichi 语言实现的三维图形变换演示程序，展示模型变换、视图变换和透视投影变换的完整流程。

## 项目简介

本次实验用代码实现模型变换、视图变换和透视投影变换的完整流程，使用 Taichi 语言实现。理解3D空间中的坐标变换流程。

## 项目架构

实验二/
├── test.py
├── .gitignore 
└── README.md   

## 运行环境

- Python 3.11+
- Taichi 1.8+

## 效果演示
![效果演示](./效果演示.gif)
按A/D键控制三角形绕Z轴旋转

## 安装依赖

```bash
# 激活虚拟环境
conda activate cg_env

# 安装 Taichi
pip install taichi