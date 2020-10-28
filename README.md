# **Have a look (**[**Live Demo**](https://www.linkedin.com/feed/update/urn:li:activity:6700769763758542848/)**) of real-time face mask detection.**

**Datasets** : [https://www.kaggle.com/andrewmvd/face-mask-detection](https://www.kaggle.com/andrewmvd/face-mask-detection)

**Label\_map** : [labelmap.pbtxt](https://github.com/hgoyal194/real-time-facemask-detection/blob/master/labelmap.pbtxt)

## **For setup and Training:**

**Local/windows:** [https://c17hawke.github.io/tfod-setup/](https://c17hawke.github.io/tfod-setup/)

**For using colab gpu for training:** [mask\_detection\_ssdlie\_tf1\_x.ipynb](https://github.com/hgoyal194/real-time-facemask-detection/blob/master/mask_detection_ssdlie_tf1_x.ipynb)</br>
Upload all the model files with train, test record files to your drive then use colab for training</br>
There are also another methods without uploading</br>

**For Live cam detection:** [mask\_detect\_live\_cam.py](https://github.com/hgoyal194/real-time-facemask-detection/blob/master/mask_detect_live_cam.py)

## Why I used ssdlite\_mobilenet\_v2\_coco model?

- After some investigation with the some models I decided to use  **ssdlite\_mobilenet\_v2\_coco** with **150k steps**  as it offers a faster speed and good [mean\_average\_precision](http://cocodataset.org/#detection-eval) (mAP).
- I also trained with **&#39;faster\_rcnn\_inception&#39; with 200k** steps and got very good accuracy but speed is very low (1 fps).

## **References:**

[https://github.com/tensorflow/models/tree/master/official](https://github.com/tensorflow/models/tree/master/official)</br>
[https://github.com/tensorflow/models/blob/master/research/object\_detection/g3doc/tf1\_detection\_zoo.md](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf1_detection_zoo.md)</br>
[https://github.com/tensorflow/models/blob/master/research/object\_detection/colab\_tutorials/object\_detection\_tutorial.ipynb](https://github.com/tensorflow/models/blob/master/research/object_detection/colab_tutorials/object_detection_tutorial.ipynb)</br>
[https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/auto\_examples/object\_detection\_camera.html#sphx-glr-auto-examples-object-detection-camera-py](https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/auto_examples/object_detection_camera.html#sphx-glr-auto-examples-object-detection-camera-py)</br>
[https://c17hawke.github.io/tfod-setup/p02/](https://c17hawke.github.io/tfod-setup/p02/)
