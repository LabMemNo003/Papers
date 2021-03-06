+ **Vision-Guided Automatic Parking for Smart Car**  
  2000 - (2019/04/03: 127) - [Ming Xie]
  - 输入图像 --> 使用RCE神经网络分割停车线 --> 拟合停车线轮廓 --> 投影至地面坐标
  - 输入图像 --> 利用双目相机检测障碍物
  - 停车路径的规划及控制命令的生成
+ **Parking Slot Markings Recognition for Automatic Parking Assist System**  
  2006 - (2019/04/03: 99) - [Ho Gi Jung] [Dong Suk Kim] [Pal Joo Yoon] [Jaihie Kim]
  - **利用 "停车线本身的宽度" 及 "两条平行停车线的距离" 作为约束, 在Hough变换的参数空间中寻找潜在停车线, 并利用空间约束进一步过滤** 
  - 后广角相机 --> 去畸变 --> Sobel边缘检测 --> Hough变换 --> 检测直线(线宽) --> 识别停车线(平行与垂直关系) --> 识别地标线段 --> 识别引导线 --> 切割地标线段 --> 识别停车位
+ **Uniform User Interface for Semiautomatic Parking Slot Marking Recognition**  
  2010 - (2019/04/03: 55) - [Ho Gi Jung] [Yun Hee Lee] [Jaihie Kim]
  - **用户提供两个点，指出停车线入口的端点, 并以此为基础检测停车位**
  - ROI; 图像二值化; 模板匹配; Distance Transform
+ **Fully-automatic Recognition of Various Parking Slot Markings in Around View Monitor(AVM) Image Sequences**  
  2012 - (2019/04/03: 20) - [Jae Kyu Suhr] [Ho Gi Jung]
  - 利用"Full-automatic recognition of various parking slot markings using a hierarchical tree structure"中的方法, 检测每一帧中的停车位
  - **计算每一帧间的homography矩阵, 并利用该矩阵预测前一帧的停车位在后一帧中的位置, 结合预测结果与后一帧的检测结果, 获取更高置信度的停车位**
+ **Full-automatic recognition of various parking slot markings using a hierarchical tree structure**  
  2013 - (2019/04/03: 33) - [Jae Kyu Suhr] [Ho Gi Jung]
  - **利用 "不同类型的停车位, 由不同的停车线连接点(junction)组成; 不同类型的停车线连接点(junction), 由不同的角点(corner)组成" 的特点, 分多个层次检测停车位**
  - 输入图像 --> Harris角点检测 --> 绕角点一周进行采样 --> 利用不同角度的模板对采样数据滤波 --> 对角点进行分类并计算方向 --> 遍历每一对角点生成可能的连接点 --> 遍历每一对连接点生成可能的停车位 --> 过滤重叠的停车位
+ **Automatic Parking Based on a Bird's Eye View Vision System**  
  2014 - (2019/04/03: 50) - [Chunxiang Wang] [Hengrun Zhang] [Ming Yang] [Xudong Wang] [Lei Ye] [Chunzhao Guo]
  - **直接在边缘提取的特征图上做Radon变换**
  - 四路鱼眼镜头 --> 去畸变 --> 鸟瞰图拼接 --> Canny边缘检测 --> Radon变换 --> 寻找高置信度的垂线 --> 提取潜在停车线 --> 聚类及过滤得到停车位 --> 检测空停车位 --> 路径规划及寻迹
+ **Line Filter-Based Parking Slot Detection for Intelligent Parking Assistance System**  
  2014 - (2019/04/03: 4) - [Mengyang Fan] [Zhengcheng Hu] [Kazukuni Hamada] [Hui Chen]
  - **使用形如[-1,-1,...,-1,-1,0,1,1,...,1,1]的卷积核, 对灰度图像进行竖直及水平方向的卷积, 从而提取直线**
  - 输入图像 --> 灰度图像 --> 用提出的卷积核进行边缘线检测 --> Hough变换及几何约束提取候选停车线 --> 基于几何约束检测停车位
+ **Surround View based Parking Lot Detection and Tracking**  
  2015 - (2019/04/03: 15) - [Kazukuni Hamada] [Zhencheng Hu] [Mengyang Fan] [Hui Chen]
  - 边缘检测 --> Hough变换提取候选线 --> 停车位检测 --> 跟踪?
+ **Directional-DBSCAN: Parking-slot Detection using a Clustering Method in Around-View Monitoring System**  
  2016 - (2019/04/03: 12) - [Soomok Lee] [Daejin Hyeon] [Gikwang Park] [Il-joo Baek] [Seong-Woo Kim] [Seung-Woo Seo]
  - **在DBSCAN中加入方向信息, 从而对提取的停车线特征进行聚类, 得到连续线段**
  - 输入全景图像 --> 使用滤波的方法提取线特征 --> 使用D-DBSCAN聚类得到线段簇 ( --> 使用linear-RANSAC判断方向一致性 ) --> 使用Sequential-RANSAC得到线段簇的方程 --> 将线段分组为不同的停车线集合 --> 判断每个停车线集合的停车位类别 --> 检测最终的停车位
+ **Available Parking Slot Recognition based on Slot Context Analysis**  
  2016 - (2019/04/03: 8) - [Soomok Lee] [Seung-Woo Seo]
  - **基于能量的聚类的过程, 其实跟Hough变换一样, 只是在参数空间沿rho方向算了一遍熵**
  - **使用Bayesian Network (BN)来判断线段组合成的潜在停车位是否合理**
  - Bayesian Network (BN) framework; Histogram of Gradient (HOG); frequency magnitude feature; Support Vector Machine (SVM)
  - 四路图像 --> 鸟瞰图 --> 停车线检测(Cone-hat Marking Extraction Filter --> Entropy-based Line-marking Clustering --> line-segment detection) --> 生成候选停车位 --> 停车位合法验证(BN model) --> 停车位是否为空(HOG, FFT, SVM)
+ **Vision-based Parking-slot detection: A Benchmark And A Learning-based Approach**  
  2017 - (2019/04/03: 6) - [Linshen Li] [Lin Zhang] [Xiyuan Li] [Xiao Liu] [Ying Shen] [Lu Xiong]
  - http://sse.tongji.edu.cn/linzhang/ps/index.htm
  - PSDL: Parking-Slot Detection based on Learning
  - **角点检测: 特征提取(normalized intensity,gradient magnitude,oriented gradient histograms) --> AdaBoost分类器**
  - 基于一些几何约束的停车位检测
+ **Vision-Based Parking-Slot Detection: A DCNN-Based Approach and a Large-Scale Benchmark Dataset**  
  2018 - (2019/04/03: 4) - [Lin Zhang] [Junhao Huang] [Xiyuan Li] [Lu Xiong]
  - https://cslinzhang.github.io/deepps/
  - DeepPS: a DCNN-based parking-slot detection approach
  - **使用YoloV2检测角点 --> 使用DCNN确定停车位类型 --> 推测停车位**
+ **Semantic Segmentation-based Parking Space Detection With Standalone Around View Monitoring System**  
  2018 - (2019/04/03: 0) - [Chulhoon Jang] [Myoungho Sunwoo]
  - 语义分割 --> 基于垂直网格的车位线检测
+ **Probabilistic Occupancy Filter for Parking Slot Marker Detection in an Autonomous Parking System Using AVM**  
  2018 - (2019/04/03: 0) - [MinChul Lee] [Seokwon Kim] [Wonteak Lim] [Myoungho Sunwoo]
  - **使用概率模型并结合连续多帧之间的联系, 减少停车位检测中由于3D物体及阴影造成的假正例**
  - Bayesian filtering scheme
+ **Vision-based Approach in Finding Multitype Parking Stall Entrance**  
  2018 - (2019/04/03: 0) - [Changmu Seo] [Joongsik Kim] [Yunhee Lee] [Whoi-Yul Kim]
  - **利用Radon变换获取候选线, 并将其交点或端点候选的停车位特征点**
  - 输入图像 --> 边缘特征提取 --> Radon变换提取候选线 --> 计算候选线间的交点坐标 --> 在交点附近做Radon变换 --> 重新计算更精确交点坐标 --> 计算交点处的停车线方向
  - 输入图像 --> 边缘特征提取 --> 边缘特征二值化 --> skeleton形态学处理 --> 获取潜在端点 --> 保留靠近车辆的端点 --> 计算端点处的停车线方向
  - --> 将靠近交点的端点过滤 --> 根据特征点的距离及角度判断停车位
  - AVM image size: 480x300; Left/right image size: 330x110; 3.75cm/pixel
+ **Geometric Features-Based Parking Slot Detection**  
  2018 - (2019/04/03: 0) - [Qian Li] [Chunyu Lin] [Yao Zhao]
  - 基于LSD的聚类算法, 检测固定间距的平行线; 使用机器学习的方法对交点进行分类, 从而确定停车线入口
  - AVM image --> ROI --> Gray image --> Morphological filter --> Edge image(Canny) --> LSD based line-clustering --> Parallel lines detection --> Parking slot generation --> Entrance Detection
