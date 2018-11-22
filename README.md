# nlp_competition
## Overview
主要使用bilstm+crf的方式搭建网络。
在特征提取上，除了常规的字向量表示外，增加了：
1. CNN提取的字组合的向量表示
2. 字所在词的位置的向量表示

* 本次采用的是在lstm中加深了网络
## Files Structures
-ckpt：保存的模型
-data：原始数据和处理好的数据
-doc：一些参考论文
-middle：一些处理的中间文件
-models：模型
-summary：tensorboard用

## Reference
Named Entity Recognition for Chinese Social Media with Jointly Trained Embeddings
Design Challenges and Misconceptions in Neural Sequence Labeling
