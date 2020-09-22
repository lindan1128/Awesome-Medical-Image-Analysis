# Awesome-Medical-Image-Analysis

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
## Background
A survey library of medical image analysis papers and codes to follow related fields quickly, as well as better and fair comparison and reproduction in research.

## Performance Table

For a fair comparison, the size of the input tensor is [1, 3, 128, 128, 128], the total levels of the network to defined as 5 (i.e., down smaple 32x) with the initial channel of 32, as level increases, the number of channels doubles.


|         ConvNet            | ImageNet top1 acc | ImageNet top5 acc |   Published In     |
|:--------------------------:|:-----------------:|:-----------------:|:------------------:|
|           Vgg              |      76.3         |       93.2        |      ICLR2015      |
|        GoogleNet           |       -           |       93.33       |      CVPR2015      |
|        PReLU-nets          |       -           |       95.06       |      ICCV2015      |
|          ResNet            |       -           |       96.43       |      CVPR2015      |
|       PreActResNet         |      79.9         |       95.2        |      CVPR2016      |
|       Inceptionv3          |      82.8         |       96.42       |      CVPR2016      |
|       Inceptionv4          |      82.3         |       96.2        |      AAAI2016      |
|    Inception-ResNet-v2     |      82.4         |       96.3        |      AAAI2016      |
|Inceptionv4 + Inception-ResNet-v2|      83.5         |       96.92       |      AAAI2016      |
|           RiR              |       -           |         -         |  ICLR Workshop2016 |
|  Stochastic Depth ResNet   |      78.02        |         -         |      ECCV2016      |
|           WRN              |      78.1         |       94.21       |      BMVC2016      |
|       SqueezeNet           |      60.4         |       82.5        |      arXiv2017([rejected by ICLR2017](https://openreview.net/forum?id=S1xh5sYgx))     |
|          GeNet             |      72.13        |       90.26       |      ICCV2017      |
|         MetaQNN            |       -           |         -         |      ICLR2017      |
|        PyramidNet          |      80.8         |       95.3        |      CVPR2017      |
|         DenseNet           |      79.2         |       94.71       |      ECCV2017      |
|        FractalNet          |      75.8         |       92.61       |      ICLR2017      |
|         ResNext            |       -           |       96.97       |      CVPR2017      |
|         IGCV1              |      73.05        |       91.08       |      ICCV2017      |
| Residual Attention Network |      80.5         |       95.2        |      CVPR2017      |
|        Xception            |       79          |       94.5        |      CVPR2017      |
|        MobileNet           |      70.6         |         -         |      arXiv2017     |
|         PolyNet            |      82.64        |       96.55       |      CVPR2017      |
|           DPN              |       79          |       94.5        |      NIPS2017      |
|        Block-QNN           |      77.4         |       93.54       |      CVPR2018      |
|         CRU-Net            |      79.7         |       94.7        |      IJCAI2018     |
|       ShuffleNet           |      75.3         |         -         |      CVPR2018      |
|       CondenseNet          |      73.8         |       91.7        |      CVPR2018      |
|          NasNet            |      82.7         |       96.2        |      CVPR2018      |
|       MobileNetV2          |      74.7         |         -         |      CVPR2018      |
|         IGCV2              |      70.07        |         -         |      CVPR2018      |
|          hier              |      79.7         |       94.8        |      ICLR2018      |
|         PNasNet            |      82.9         |       96.2        |      ECCV2018      |
|        AmoebaNet           |      83.9         |       96.6        |      arXiv2018     |
|          SENet             |       -           |       97.749      |      CVPR2018      |
|       ShuffleNetV2         |      81.44        |         -         |      ECCV2018      |
|          IGCV3             |      72.2         |         -         |      BMVC2018      |
|         MnasNet            |      76.13        |       92.85       |      CVPR2018      |
|          SKNet             |      80.60        |         -         |      CVPR2019      |
|          DARTS             |      73.3         |       91.3        |      ICLR2019      |
|       ProxylessNAS         |      75.1         |       92.5        |      ICLR2019      |
|       MobileNetV3          |      75.2         |         -         |      arXiv2019     |
|          Res2Net           |      79.2         |       94.37       |      arXiv2019     |
|       EfficientNet         |      84.3         |       97.0        |      ICML2019      |




## Performance Table

For simplicity reason, I only listed the best top1 and top5 accuracy on ImageNet from the papers. Note that this does not necessarily mean one network is better than another when the acc is higher, cause some networks are focused on reducing the model complexity instead of improving accuracy, or some papers only give the single crop results on ImageNet, but others give the model fusion or multicrop results.

- ConvNet: name of the covolution network
- ImageNet top1 acc: best top1 accuracy on ImageNet from the Paper
- ImageNet top5 acc: best top5 accuracy on ImageNet from the Paper
- Published In: which conference or journal the paper was published in.

|         ConvNet            | ImageNet top1 acc | ImageNet top5 acc |   Published In     |
|:--------------------------:|:-----------------:|:-----------------:|:------------------:|
|           Vgg              |      76.3         |       93.2        |      ICLR2015      |
|        GoogleNet           |       -           |       93.33       |      CVPR2015      |
|        PReLU-nets          |       -           |       95.06       |      ICCV2015      |
|          ResNet            |       -           |       96.43       |      CVPR2015      |
|       PreActResNet         |      79.9         |       95.2        |      CVPR2016      |
|       Inceptionv3          |      82.8         |       96.42       |      CVPR2016      |
|       Inceptionv4          |      82.3         |       96.2        |      AAAI2016      |
|    Inception-ResNet-v2     |      82.4         |       96.3        |      AAAI2016      |
|Inceptionv4 + Inception-ResNet-v2|      83.5         |       96.92       |      AAAI2016      |
|           RiR              |       -           |         -         |  ICLR Workshop2016 |
|  Stochastic Depth ResNet   |      78.02        |         -         |      ECCV2016      |
|           WRN              |      78.1         |       94.21       |      BMVC2016      |
|       SqueezeNet           |      60.4         |       82.5        |      arXiv2017([rejected by ICLR2017](https://openreview.net/forum?id=S1xh5sYgx))     |
|          GeNet             |      72.13        |       90.26       |      ICCV2017      |
|         MetaQNN            |       -           |         -         |      ICLR2017      |
|        PyramidNet          |      80.8         |       95.3        |      CVPR2017      |
|         DenseNet           |      79.2         |       94.71       |      ECCV2017      |
|        FractalNet          |      75.8         |       92.61       |      ICLR2017      |
|         ResNext            |       -           |       96.97       |      CVPR2017      |
|         IGCV1              |      73.05        |       91.08       |      ICCV2017      |
| Residual Attention Network |      80.5         |       95.2        |      CVPR2017      |
|        Xception            |       79          |       94.5        |      CVPR2017      |
|        MobileNet           |      70.6         |         -         |      arXiv2017     |
|         PolyNet            |      82.64        |       96.55       |      CVPR2017      |
|           DPN              |       79          |       94.5        |      NIPS2017      |
|        Block-QNN           |      77.4         |       93.54       |      CVPR2018      |
|         CRU-Net            |      79.7         |       94.7        |      IJCAI2018     |
|       ShuffleNet           |      75.3         |         -         |      CVPR2018      |
|       CondenseNet          |      73.8         |       91.7        |      CVPR2018      |
|          NasNet            |      82.7         |       96.2        |      CVPR2018      |
|       MobileNetV2          |      74.7         |         -         |      CVPR2018      |
|         IGCV2              |      70.07        |         -         |      CVPR2018      |
|          hier              |      79.7         |       94.8        |      ICLR2018      |
|         PNasNet            |      82.9         |       96.2        |      ECCV2018      |
|        AmoebaNet           |      83.9         |       96.6        |      arXiv2018     |
|          SENet             |       -           |       97.749      |      CVPR2018      |
|       ShuffleNetV2         |      81.44        |         -         |      ECCV2018      |
|          IGCV3             |      72.2         |         -         |      BMVC2018      |
|         MnasNet            |      76.13        |       92.85       |      CVPR2018      |
|          SKNet             |      80.60        |         -         |      CVPR2019      |
|          DARTS             |      73.3         |       91.3        |      ICLR2019      |
|       ProxylessNAS         |      75.1         |       92.5        |      ICLR2019      |
|       MobileNetV3          |      75.2         |         -         |      arXiv2019     |
|          Res2Net           |      79.2         |       94.37       |      arXiv2019     |
|       EfficientNet         |      84.3         |       97.0        |      ICML2019      |


## Papers&Codes