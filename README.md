Using convolutional neural network for multi-label multi-class classification
	
## Dataset
The [image dataset](https://www.lamda.nju.edu.cn/data_MIMLimage.ashx) consists of 2000 natural scene images, where a set of labels is artificially assigned to each image

## Approach
[notebook](https://github.com/bhavikfirke/Multilabel_Image_Classification/blob/main/scene_label_github.ipynb)
### Preprocessing
- Due to small dataset, image augmentation was used to artifically increase training data
### Training
- Used a sequential CNN architecture along with dropout and batch normalization layers to avoid overfitting
- As this was multi label classification, binary crossentropy and sigmoid was used as loss function and activation function respectively
- To select threshold value, performance of various threshold values was evaluated using Matthews Correlation Coefficient

### Model Architecture
![model](https://github.com/bhavikfirke/Multilabel_Image_Classification/blob/main/model.png?raw=true)

## Outcome
- Obtained 0.12 Hamming loss on test set
- Obtained 59% exact match on test set

### Predictions on test set
![sample_test_image](https://github.com/bhavikfirke/Multilabel_Image_Classification/blob/main/test_image.jpg?raw=true)
