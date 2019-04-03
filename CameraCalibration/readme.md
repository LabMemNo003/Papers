+ **A Flexible New Technique for Camera Calibration**  
  1998 - (2019/04/03: 12202) - [Zhengyou Zhang]
  - 利用多张不同角度的棋盘格照片进行标定, 不需要确定棋盘格位置, 非广角镜头
+ **Estimation of omnidirectional camera model from epipolar geometry**  
  2003 - (2019/04/03: 193) - [Branislav Micucik] [Tomas Pajdla]
  - Scaramuzza标定法的引用文献之一, Scaramuzza采用了与该文献相同的变量名和坐标系
  - 复杂的全景相机模型 --> 模型化简 --> 模型线性化 --> 模型求解
+ **A Flexible Technique for Accurate Omnidirectional Camera Calibration and Structure from Motion**  
  2006 - (2019/04/03: 385) - [Davide Scaramuzza] [Agostino Martinelli] [Roland Siegwart]
  - 图像坐标系(u,v) --> 相机坐标系(u,v,f(x)) --> 世界坐标系(x,y,z)
  - 假设光轴与成像面垂直(局限); 假设标定用的平面z=0, 以简化模型
  - 以光轴为中心建立极坐标系; 用多项式f(x)扩展极坐标系, 建立球面坐标系; 利用外参换算世界坐标
  - 论文中(7)式的叉乘是求解过程的重点
  - 先求解得到外参中的r11, r12, r21, r22, r31, r32, t1, t2等外参(t3除外); 后求解得到t3及f(x)中的内参
+ **A Toolbox for Easily Calibrating Omnidirectional Cameras**  
  2006 - (2019/04/03: 515) - [Davide Scaramuzza] [Agostino Martinelli] [Roland Siegwart]
  - 提供了Scaramuzza标定法工具箱
  - 求解外参 --> 求解内参 --> 线性优化内外参 --> 迭代寻找图像中心 --> 非线性优化
+ **A Generic Camera Model and Calibration Method for Conventional, Wide-Angle, and Fish-Eye Lenses**  
  2006 - (2019/04/03: 549) - [Juho Kannala] [Sami S. Brandt]
  - 与Scaramuzza标定法的思想类似, 利用多项式来拟合光路的投影偏角
  - 考虑了径向畸变与切向畸变, 即不要求光轴必须垂直于成像面, 但模型更加复杂
+ **Automatic Detection of Checkerboards on Blurred and Distorted Images**  
  2008 - (2019/04/03: 120) - [Martin Rufli] [Davide Scaramuzza] [Roland Siegwart]
  - 用于在畸变图中自动检测棋盘格, 被加入到Scaramuzza标定法工具箱中
  - 图像输入 --> 二值化 --> 腐蚀 --> 检测四边形 --> 链接四边形 --> 确定角点顺序
