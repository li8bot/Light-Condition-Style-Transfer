# Light Conditions Style Transfer

## Paper
Lane Detection in Low-light Conditions Using an Efficient Data Enhancement : Light Conditions Style Transfer

Submit : IV 2020

The main framework is as follows:
![Our framework](https://github.com/Chenzhaowei13/Light-Condition-Style-Transfer/blob/master/data/framework.png)

## Source Code

1. Better-CycleGAN

We will open the source code for Better-CycleGAN soon.

2. ERFNet

The source code used for the lane detction is made publicly available by [HOU Yuenan](https://github.com/cardwing/Codes-for-Lane-Detection/tree/master/ERFNet-CULane-PyTorch)

## Datasets

### CULane

The whole dataset is available at [CULane](https://xingangpan.github.io/projects/CULane.html).

### Generated Images

The  images in low-light conditions are generated by the proposed Better-CycleGAN.  We will upload our generated images in low-light conditions soon.


## Trained model

The trained models used in this paper are available in ./trained


## Performance

1. Light-Conditions transfer

Some examples of real images in normal light conditions and their corresponding translations images in low-light conditions.
![images](https://github.com/Chenzhaowei13/Light-Condition-Style-Transfer/blob/master/data/transfer_result.png)


2. Lane detetcion

Performance ( (F<sub>1</sub>-measure) ) of different methods on CULane testing set. For crossroad, only FP is shown.

| Category | ERFNet | CycleGAN+ERFNet | Better-CycleGAN+ERFNet(ours) | SCNN | ENet-SAD | ResNet-101-SAD |
|:----:|:----:|:----:|:----:|:----:|:----:|:----:|
| Normal | 91.5 | 91.7 | 91.8 | 90.6 | 90.1 | 90.7 |
| Crowded | 71.6 | 71.5 | 71.8 | 69.7 | 68.8 | 70.0 |
| Night | 67.1 | 68.9 | 69.4 | 66.1 | 66.0 | 66.3 |
| No Line | 45.1 | 45.2 | 46.1 | 43.4 | 41.6 | 43.5 |
| Shadow | 71.3 | 73.1 | 76.2 | 66.9 | 65.9 | 67.0 |
| Arrow | 87.2 | 87.2 | 76.2 | 66.9 | 65.9 | 67.0 |
| Dazzle Light | 66.0 | 67.5 | 66.4 | 58.5 | 60.2 | 59.9 |
| Curve | 71.6 | 69.0 | 72.4 | 64.4 | 65.7 | 65.7 |
| Crossroad | 2199 | 2402 | 2346 | 1990 | 1998 | 2052 |
| Total | 73.1 | 73.6 | 73.9 | 71.6 | 70.8 | 71.8 |

The probability maps output by the three methods above are shown as following
![images](https://github.com/Chenzhaowei13/Light-Condition-Style-Transfer/blob/master/data/lane_detection_results.png)


## To do

- Upload the generated images

- Open the source code for Better-CycleGAN

## Acknowledgement

This project refers to the following projects:

-  [Codes-for-Lane-Detection](https://github.com/cardwing/Codes-for-Lane-Detection)
-  [SCNN](https://github.com/XingangPan/SCNN)






