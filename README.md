# WRS2018_dataset

YOLO dataset for WRS 2018 (world robot summit - partner robot challenge in real space)

We participated in WRS 2018 and we used YOLO to recognize target objects.
This dataset is used there and used for training the YOLO v3.
The objects can be shown [here](https://github.com/wrs-prc-realspace/WRS2018Tokyo/blob/master/known_objects.md).
The detailed labels of each object are as below and some objects which seem like that HSR cannot grasp are not annotated.

```
0	Dog plush toy
1	Rabbit plush toy
2	Hedgehog plush toy
	Postcard with moon image
	Postcard with temple image
	Postcard with waterfall image
3	Bus toy car
4	Fire engine toy car
5	Police toy car
6	Whistle sound toy
7	Shaker sound toy
8	Horn sound toy
9	Cube block
10	Triangular block
11	Cylinder block
12	Wooden Bowl
	Brown pail
13	Mixed nuts
14	Blue cup
15	Pink cup
16	Orange biscuits
17	Yellow biscuits
	Watering can
18	Flashlight
19	Blue fork
20	Green spoon
21	Gray knife
22	Pink biscuits
23	Yellow clock
24	Aluminum foil
25	Green dish
26	Yellow dish
27	Pink bowl
28	Blue bowl
29	Mineral water
30	Oolong Tea
31	Ketchup
32	Canned mustard
33	Orange drink
34	Green drink
35	Tomato
36	Potato
37	Plant
38	Spray
39	Water bottle
40	Blueberry drink
41	Eggplant
```


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

The dataset have 2 datasets. One is composed of real images and the other is composed of synthesize images.
Annotaion style follows the annotation style of YOLO. Therefore, you can use it directly for training YOLO.

Real images are taken by several cameras such as phone cameras, RealSense D435, and Xtion. The objects are
placed at random sites in the demonstration place.

Synthesized images are generated by combining a background image and several object images. The background image
is selected from ~100 background image candidates which collected by web crawling and taken around the target envrionment. 
The object images are taken in a studio and the background is eliminated. These object images are taken for all objects.

Dataset link: https://drive.google.com/file/d/1Tq9hKbqKrnTmpaMFzO3Ewt2Hocz8JT75/view?usp=sharing

This dataset is published under the LGPL license.
