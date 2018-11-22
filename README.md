# nlp_competition
## Overview
本次比赛是nlp中命名实体识别的相关比赛。本次比赛需要设计算法来对糖尿病相关的教科书、研究论文来进行实体标注构建。
个人成绩：0.6720，第一名成绩：0.763  

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
--bilstm_cnn_crf: 加入CNN提取特征的模型  
---network  
---train  
---prediction  
--bilstm_crf：bi lstm crf  
---network  
---train  
---prediction  
-summary：tensorboard用  
-data_process：数据处理，包括oversampling  
-tools：未分类的tools  

## Reference
Named Entity Recognition for Chinese Social Media with Jointly Trained Embeddings  
Design Challenges and Misconceptions in Neural Sequence Labeling  
