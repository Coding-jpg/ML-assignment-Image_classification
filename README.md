# ML-assignment-Image_classification
An assignment of machine learning.
data source: 


### Task
图像分类
数据集：OrganCMNIST
选用模型SVM，MLP（FCNN），CNN

### 数据探索（data exploration）
1. 数据规模及图像尺寸
2. 缺失值检查
3. 每个类别包含多少数据，是否均衡（不均衡，新增混淆矩阵作为评价标准之一）
4. 单一图像展示
5. 类别特征相似性（少量特征相似，采用图像增强）

### 数据预处理
1. 标签数据one-hot编码（只作用于MLP和CNN）
2. 数据reshape（只作用于MLP和CNN）
3. 特征提取（只作用于LinearSVC）
4. 数据增强（在后面Data Enhance）：旋转、2个方向拉伸、标准化、缩放。

### 模型建立及训练
1. LinearSVC：用accuracy、precision、recall、f1作为评价指标
2. MLP: 用accuracy、confusion matrix作为评价指标，FCNN()用于建立单一模型，FCNN_tuning()用于参数搜索过程中建立模型
3. CNN：用accuracy、confusion matrix 作为评价指标，CNN()用于建立单一模型，
CNN_tuning()用于参数搜索过程中建立模型

### 参数搜索(每个部分都根据最优参数获得一个最好模型)
1. LinearSVC：GridSearch
2. MLP & CNN：RandomSearch
