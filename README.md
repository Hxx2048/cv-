# cv-进度
主要用来记录作业进度，这是一个跨媒体检索的框架，基础框架为DAN, 改进text encoder为BERT，image encoder为Mask RCNN.
![image](https://github.com/Hxx2048/cv-/blob/master/framework.PNG)

# 目前进度
2018/12/20      BERT, DAN代码跑通,下一步跑tf版本的maskRCNN

# Reference
[Mask R-CNN](https://arxiv.org/pdf/1703.06870.pdf)<br>
[BERT: Pre-training of Deep Bidirectional Transformers for Language Understanding](https://arxiv.org/pdf/1810.04805.pdf)<br>
[Dual Attention Networks for Multimodal Reasoning and Matching](https://arxiv.org/pdf/1611.00471.pdf)<br>

# Code
DualAttentionNetwork:<br>
[https://github.com/google-research/bert](https://github.com/google-research/bert)  mDAN, tf实现，可复现，效果不是很好<br>
[https://github.com/kelelexu/pytorch-vqa-dan](https://github.com/kelelexu/pytorch-vqa-dan)  rDAN, torch版本,需修改为mDAN<br>

BERT：<br>
[https://github.com/google-research/bert](https://github.com/google-research/bert) tf版本，可使用<br>

MaskRCNN:<br>
[https://github.com/CharlesShang/FastMaskRCNN](https://github.com/CharlesShang/FastMaskRCNN ) tf版本<br>
1. Go to ./libs/datasets/pycocotools and run make
2. Download COCO dataset, place it into ./data, then run python download_and_convert_data.py to build tf-records. It takes a while.[>12h]
3. Download pretrained resnet50 model, wget http://download.tensorflow.org/models/resnet_v1_50_2016_08_28.tar.gz, unzip it, place it into ./data/pretrained_models/
4. Go to ./libs and run make
5. run python train/train.py for training



# Dataset
[COCO](http://cocodataset.org/#download)
