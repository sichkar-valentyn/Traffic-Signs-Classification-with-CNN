# Traffic Signs Classification with CNN
Implementing CNNs for effective Traffic Signs classification.
<br/>[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3605407.svg)](https://doi.org/10.5281/zenodo.3605407)


### Related Paper
Sichkar V. N., Kolyubin S. A. Effect of various dimension convolutional layer filters on traffic sign classification accuracy. Scientific and Technical Journal of Information Technologies, Mechanics and Optics, 2019, vol. 19, no. 3, pp. DOI: 10.17586/2226-1494-2019-19-3-546-552 (Full-text available also <a href="https://www.researchgate.net/publication/334074308_Effect_of_various_dimension_convolutional_layer_filters_on_traffic_sign_classification_accuracy" target="_blank">here</a>)

### :mortar_board: Related Course for Detection Tasks
**Training YOLO v3 for Objects Detection with Custom Data.** *Build your own detector by labelling, training and testing on image, video and in real time with camera.* Available here: [https://www.udemy.com/course/training-yolo-v3-for-objects-detection-with-custom-data/](https://www.udemy.com/course/training-yolo-v3-for-objects-detection-with-custom-data/?referralCode=A283956A57327E37DDAD)

Detections on video are shown below. **Trained weights** for detection tasks can be found in the course mentioned above.
![Detections on Video](https://www.googleapis.com/download/storage/v1/b/kaggle-user-content/o/inbox%2F3400968%2F11bee8c0918c092b7d256b5254ba441c%2Fts_detections.gif?generation=1581794210627123&alt=media "Detections of Traffic Signs on Video")

Explore dataset used for training and detection tasks here: [https://www.kaggle.com/valentynsichkar/traffic-signs-dataset-in-yolo-format](https://www.kaggle.com/valentynsichkar/traffic-signs-dataset-in-yolo-format)

### :triangular_flag_on_post: Concept Map of the Course
![Concept Map of the Course](https://github.com/sichkar-valentyn/YOLO-v3-Objects-Detection-with-Custom-Data/blob/master/images/Concept_map_YOLO_3.png "Concept Map of the Course")

### :point_right: Join the Course
[https://www.udemy.com/course/training-yolo-v3-for-objects-detection-with-custom-data/](https://www.udemy.com/course/training-yolo-v3-for-objects-detection-with-custom-data/?referralCode=A283956A57327E37DDAD)

<br/>

### Content
* [Description](#description)
* [How to use](#how-to-use)
* [Results](#results)

<br/>

### <a id="description">Description</a>
Experimenting with different dimensions of Convolutional Neural Network's **Filters** in order to find the most accurate solution for Traffic Signs Classification.

<br/>

### <a id="how-to-use">How to use</a>
- [x] The easiest way is to clone code on **Kaggle** <a href="https://www.kaggle.com/valentynsichkar/traffic-signs-classification-with-cnn" target="_blank">here</a>.
- [x] Another option would be to download **Jupyter Notebook** file and use it at local machine. But in this case, you need to download also dataset that is located on **Kaggle** <a href="https://www.kaggle.com/valentynsichkar/traffic-signs-preprocessed" target="_blank">here</a>. Also, change the location of **dataset** in the second cell, pointing to the downloaded file, e.g.:
```py
# Opening file for reading in binary mode
with open('../input/traffic-signs-preprocessed/data2.pickle', 'rb') as f:
    data = pickle.load(f, encoding='latin1')  # dictionary type
```

<br/>

### <a id="results">Results</a>
Find below training results for Traffic Signs classification by CNNs.

Model's filters  | Training Accuracy | Validation Accuracy
------------- | ------------- | -------------
3x3  | 0.98792 | 0.86440
5x5  | 0.98568 | 0.88594
9x9  | 0.98049 | 0.86576
13x13  | 0.97101 | 0.83152
15x15  | 0.96905 | 0.84444
19x19  | 0.96085 | 0.83107
23x23  | 0.94966 | 0.83946
25x25  | 0.94912 | 0.84172
31x31  | 0.93354 | 0.83311

On the Figure below graph is shown for different Model's filters.
<br/>

![Accuracy of different Models filters](https://github.com/sichkar-valentyn/Traffic-Signs-Classification-with-CNN/blob/master/accuracy.png "Accuracy of different Models filters")

On the Figure below trained filters are shown for 31x31 Model.
<br/>

![Trained filters for 31x31 Model](https://github.com/sichkar-valentyn/Traffic-Signs-Classification-with-CNN/blob/master/filters31x31.png "Trained filters for 31x31 Model")

<br/>

### MIT License
### Copyright (c) 2020 Valentyn N Sichkar
### github.com/sichkar-valentyn
### Reference to:
Valentyn N Sichkar. Traffic Signs Classification with CNN // GitHub platform. DOI: 10.5281/zenodo.3605407
