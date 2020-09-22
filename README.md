# Awesome-Medical-Image-Analysis

[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
## Background
A survey library of medical image analysis papers and codes to follow related fields quickly, as well as better and fair comparison and reproduction in research.

## Performance Table

For a fair comparison, the size of the input tensor is [1, 3, 128, 128, 128], the total levels of the network is defined as 5 (i.e., down smaple 32x) with the initial channel of 32, as level increases, the number of channels doubles. 
If not special specified, the network adopts Batch Normlization and RELU operator by defailt.


|         Network            |     Params        |       Flops       |
|:--------------------------:|:-----------------:|:-----------------:|:------------------:|
|                         |      76.3         |       93.2        |      ICLR2015      |


