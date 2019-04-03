+ **A Combined Corner And Edge Detector**  
  1988 - (2019/04/03: 16019) - [Chris Harris] [Mike Stephens]
  - Harris角点检测, 从Moravec角点检测改进而来
  - 使用图像强度对x及y方向的一阶偏导, 而非简单差值, 来计算任意方向偏移变化
  - 使用高斯函数作为窗口函数, 而非二值的矩形, 从而提高对噪声的鲁棒性
  - 将评价函数写为矩阵相乘的形式, 利用二次型矩阵的特征值, 来判断是否为角点或边
