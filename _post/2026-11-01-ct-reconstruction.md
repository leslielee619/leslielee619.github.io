---
title: "CT图像重建中的一些思考"

date: 2026-11-01 10:00:00 +0800

categories:
  - CT
  - Reconstruction

tags:
  - Radon Transform
  - FBP
  - Image Reconstruction

---

# 1. Introduction

CT图像重建是计算机断层成像的核心问题之一。

从数学上看，CT重建可以理解为由投影数据恢复
物体内部二维或三维分布的逆问题。

<!--more-->

# 2. Mathematical Model

设二维物体分布为：

\[
f(x,y)
\]

其 Radon 变换定义为：

\[
p(\theta,s)
=
\int_{-\infty}^{+\infty}
f(s\cos\theta-t\sin\theta,
s\sin\theta+t\cos\theta)
dt
\]

# 3. Reconstruction

经典的解析重建方法包括：

- Filtered Back Projection
- Fourier Reconstruction

# 4. Python Implementation

```python
import numpy as np

def reconstruction_example(data):

    image = np.asarray(data)

    return image
