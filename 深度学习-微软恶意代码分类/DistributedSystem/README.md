课题1：微软恶意代码分类
说在前面：
示例文件中的randomsubset.py文件用于从全部数据集中随机提取一部分，作为子集，训练集和数据集，但是由于目前
得到的用于操作的数据已经是子集，所以此文件不必运行。
csv文件夹里面存放的是提取的各类特征的.csv文件
代码说明：
DrawASMFileImageFeature.py
提取ASM文件图像纹理特征
DrawOpcode_n-gramFeature.py
提取恶意代码文件opcode—n-gram特征
ImgfeaturePrediction_800pixel.py
基于ASM文件图像纹理800像素特征的随机森林、支持向量分类、核支持向量分类、朴素贝叶斯分类、逻辑回归、决策树、
GBDT（梯度提升树）算法实现模型训练和分类预测；以及使用tensorflow实现两层神经网络模型训练和分类预测
ImgfeaturePrediction_1500pixel.py
基于ASM文件图像纹理1500像素特征的随机森林、支持向量分类、核支持向量分类、朴素贝叶斯分类、逻辑回归、决策树、
GBDT（梯度提升树）算法实现模型训练和分类预测；以及使用tensorflow实现两层神经网络模型训练和分类预测
ImgfeaturePrediction_2500pixel.py
基于ASM文件图像纹理2500特征的随机森林、支持向量分类、核支持向量分类、朴素贝叶斯分类、逻辑回归、决策树、
GBDT（梯度提升树）算法实现模型训练和分类预测；以及使用tensorflow实现两层神经网络模型训练和分类预测
NGramfeaturePrediction_2.py
基于opcode-2-gram特征的随机森林、支持向量分类、核支持向量分类、朴素贝叶斯分类、逻辑回归、决策树、
GBDT（梯度提升树）算法实现模型训练和分类预测
NGramfeaturePrediction_3.py
基于opcode-3-gram特征的随机森林、支持向量分类、核支持向量分类、朴素贝叶斯分类、逻辑回归、决策树、
GBDT（梯度提升树）算法实现模型训练和分类预测
NGramfeaturePrediction_4.py
基于opcode-4-gram特征的随机森林、支持向量分类、核支持向量分类、朴素贝叶斯分类、逻辑回归、决策树、
GBDT（梯度提升树）算法实现模型训练和分类预测
CombinePrediction.py
基于ASM文件图像纹理800特征和opcode-2-gram特征、ASM文件图像纹理800特征和opcode-3-gram特征、
ASM文件图像纹理800特征和opcode-4-gram特征、ASM文件图像纹理1500特征和opcode-2-gram特征、
ASM文件图像纹理1500特征和opcode-3-gram特征、ASM文件图像纹理2500特征和opcode-4-gram特征、
ASM文件图像纹理2500特征和opcode-2-gram特征、ASM文件图像纹理2500特征和opcode-3-gram特征、
ASM文件图像纹理2500特征和opcode-4-gram特征的随机森林、支持向量分类、核支持向量分类、朴素贝叶斯分类、
逻辑回归、决策树、GBDT（梯度提升树）算法实现模型训练和分类预测
BestPrediction.py
基于ASM文件图像纹理2500像素特征，使用两层神经网络实现最优预测结果
运行说明：
1.提取特征的文件将提取的特征存放在csv文件夹下，而csv文件夹在工程目录，所以不必更改代码运行路径；
2.命令行运行Run.sh文件，耐心等待即可看到所有结果