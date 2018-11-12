# CRNN.pytorch
## Introduction
This is a pytorch implementation of [An End-to-End Trainable Neural Network for Image-based Sequence Recognition and Its Application to Scene Text Recognition](https://arxiv.org/abs/1507.05717).<br>
This implementation is similar to [https://github.com/meijieru/crnn.pytorch](https://github.com/meijieru/crnn.pytorch), we rewrite it and make it easy to understand.
## Requirements
1. Pytorch >= 0.4.0 <br>
2. opencv <br>
3. [warp_ctc_pytorch](https://github.com/SeanNaren/warp-ctc)
4. tqdm
## Construct dataset
The names of train and val data are constructed as bellow:
```
img_xxx_$$$.jpg
```
where 'xxx' represents the number of this image and '$$$' represents the label of this image. For example，‘img_0_WHLU.jpg’. <br>
![img_0_WHLU](https://github.com/jingjing-you/GRCNN.pytorch/blob/master/data_sample/img_0_WHLU.jpg)<br>
Other examples are in `data_sample` directory.

## Training the model 
You can run `python train.py` to train your model.
## Evaluation
You can run `python eval.py` to eval your model.
## References
1. [https://github.com/meijieru/crnn.pytorch](https://github.com/meijieru/crnn.pytorch) <br>
2. [https://github.com/bgshih/crnn](https://github.com/bgshih/crnn) <br>
