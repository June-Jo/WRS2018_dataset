# WRS2018_dataset

YOLO dataset for WRS 2018 (world robot summit - partner robot challenge in real space)

We participated in WRS 2018 and we used YOLO to recognize target objects.
This dataset is used there and used for training the YOLO v3.
The objects can be shown [here](https://github.com/wrs-prc-realspace/WRS2018Tokyo/blob/master/known_objects.md).
The structure of each dataset is as follows.

```
   |- Dataset
   |--- Dataset 1 (real images)
   |------- JPEGImages
   |---------- xxxxx.jpg(or other image extensions)
   |------- Labels
   |---------- xxxxx.txt
   | 
   |--- Dataset 2 (synthesized images)
   |------- JPEGImages
   |---------- xxxxx.jpg(or other image extensions)
   |------- Labels
   |---------- xxxxx.txt
```

The dataset have 2 sets of dataset. One is composed of real images and the other is composed of synthesize images.
Annotaion style follows the annotation style of YOLO. Therefore, you can use it directly for training YOLO.

Dataset link: https://drive.google.com/file/d/1Tq9hKbqKrnTmpaMFzO3Ewt2Hocz8JT75/view?usp=sharing

This dataset is published under the LGPL license.
