# 贝塞尔曲线可视化程序

## 项目简介

本项目使用 **Taichi** 和 **NumPy** 实现了一个高性能的贝塞尔曲线交互式可视化程序。通过 **De Casteljau** 算法动态生成贝塞尔曲线，并利用 GPU 并行计算实现流畅的实时渲染（60 FPS）。

## 主要特性

鼠标左键点击添加控制点，实时更新贝塞尔曲线
GPU 加速渲染。利用 Taichi Kernel 在 GPU 上并行绘制曲线像素点
实时可视化：
 红色圆点：控制点位置
 绿色曲线：贝塞尔曲线（高精度 1000 个采样点）
 灰色连线：控制点之间的连线
 按 `C` 键清空所有控制点
 优化数据传输，避免 CPU-GPU 频繁通信保证高帧率

## 环境配置

### 使用 Conda

```bash
# 创建虚拟环境
conda create -n cg_env python=3.12 -y

# 激活环境
conda activate cg_env

# 安装依赖
pip install taichi numpy
```

## 代码结构
贝塞尔曲线.py
├── de_casteljau()          # CPU 端曲线计算
├── clear_pixels()          # GPU 清屏 Kernel
├── draw_curve_kernel()     # GPU 曲线绘制 Kernel
└── main()                  # 主循环与 GUI 交互

# 效果演示
！[效果演示](./贝塞尔曲线演示.gif)
