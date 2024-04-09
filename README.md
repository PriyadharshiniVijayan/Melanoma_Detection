# Melanoma Detection
>  To build a CNN based model which can accurately detect melanoma skin cancer.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)


## General Information
- Melanoma is a type of cancer that can be deadly if not detected early
- It accounts for 75% of skin cancer deaths.
- A model that can evaluate images and alert dermatologists about the presence of melanoma


## Conclusions
- The data is divided into training and validation set along with resizing the images
- The image went through scaling. As it is an RGB image,(image/255) approach is applied
- A model is built uing the rescaled images and basic layers. It had around 80% of training accuracy and 50% of validation acuuracy
- The model was clearly overfitting
- To control overfitting dropout technique was used along with data augumentation.
- The revised model gave around 50% training and validation accuracy
- On further analysis, heavy class imbalance was found. 'actinic keratosis','dermatofibroma', 'seborrheic keratosis', 'squamous cell carcinoma', 'vascular lesion' classes had comparitively very less train data
- This issue was resolved by using Augumentor technique. 500 sample datas were added to all the classes to reduce imbalance
- In the final model rescaling, augumentation and dropout techniques were included
- The final model showed a drastic increase in training and validation accuracy more thatn 80%
- The dropout and augumentation techniques helped in controlling overfitting
- Augumentor is usd to neutralize class imbalance risk
- All these factors contributed to building a more accurate model