# Python
Python基本使用

## Python中类的定义
```
class 类名：
  def __init__(self, 参数, ...): # 构造函数
    ...
  def 方法名1（self, 参数， ...): #方法1
    ...
  def 方法名2(self, 参数，  ...): #方法2
    ...
```

## NumPy
### 导入NumPy库
```
import numpy as np
```
### 生成NumPy数组
```
arr = np.array([1.0, 2.0, 3.0])
```
### 生成N维数组
生成二维数组（矩阵）：
```
A = np.array([[1, 2], [2,4]])

```
## Matplotlib
### 绘制图形
```
import numpy as np
import matplotlib.pyplot as plt
# 生成数据
x = np.arange(0, 6, 0.1)
y = np.sin(x)
# 绘制图形
plt.plot(x, y)
plt.show()
```
### pyplot的功能
在sin的图形中追加cos函数，添加标题，x轴标签等
```
x = np.arange(0, 6, 0.1)
y1 = np.sin(x)
y2 = np.cos(x)
plt.plot(x, y1, label="sin")
plt.plot(s, y2, linestyle=="--", label="cos")
plt.xlabel("x")
plt.ylabel("y")
plt.title("sin & cos")
plt.legend()
plt.show()
```

### 显示图像
from matplotlib.image import imread
img = imread("lena.png")
plt.imshow(img)
plt.show()
