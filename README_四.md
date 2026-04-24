# Phong 光照模型

一个使用Taichi语言实现的实时 Phong 光照模型演示程序，展示了球体和圆锥体的光线追踪渲染，并支持动态调整材质参数。

## 项目简介
本项目使用Taichi高性能并行计算语言，实现了经典 Phong 光照模型的光线追踪渲染器。通过 GPU 加速，实现实时交互的 3D 图形渲染演示。
包含环境光、漫反射光、高光分量实现，球体和圆锥体表面计算，滑块动态调整材质属性。

## 运行环境
python 3.13+
Taichi 1.7+

## 安装依赖

```bash
# 激活虚拟环境
conda activate cg_env

# 安装 Taichi
pip install taichi


## 效果演示

![Demo](光照模型演示.gif)
