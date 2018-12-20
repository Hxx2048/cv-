# cv-进度
主要用来记录作业进度，这是一个跨媒体检索的框架，基础框架为DAN,改进text encoder为BERT，image encoder为Mask RCNN.
![image](https://github.com/Hxx2048/cv-/blob/master/framework.PNG)

# 目前进度
2018/12/20  BERT,DAN代码跑通,下一步跑tf版本的maskRCNN

# Reference
[Mask R-CNN](https://arxiv.org/pdf/1703.06870.pdf)
        [BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/pdf/1810.04805.pdf)    [Dual Attention Networks for Multimodal Reasoning and Matching](https://arxiv.org/pdf/1611.00471.pdf)

# Code
DualAttentionNetwork:   [https://github.com/google-research/bert](https://github.com/google-research/bert) mDAN, tf实现，可复现，效果不是很好
    [https://github.com/kelelexu/pytorch-vqa-dan](https://github.com/kelelexu/pytorch-vqa-dan) rDAN, torch版本,需修改

BERT：
    [https://github.com/google-research/bert](https://github.com/google-research/bert) tf版本，可使用

MaskRCNN:
    需要tf版本，实现三份代码的对接

# Dataset
COCO/filk30

