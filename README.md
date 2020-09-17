# Mask Detection Integration with Instagram

Rudy Wang

## Background

As schools/universities reopen and younger people are going back to school, we need to be even more vigilant in wearing our masks appropriately to curb further coronavirus impact on our communities. 

Through social media, we would be able to reach out to a younger audience base and promote mask-wearing habits as a social norm. 

## Mission

My focus is to develop a mask classifier application using computer vision and integrate it with Instagram to promote mask awareness in the younger generation.

## Process

1. Downloaded the image datasets that I will be training my neural network on - binary image classification between pictures of faces with masks, and faces without masks. For my non-mask images, I used the [Labeled Faces in the Wild Dataset](http://vis-www.cs.umass.edu/lfw/). As for my masked images, I used two datasets: [Real World Masked Face Dataset](https://github.com/X-zhangyang/Real-World-Masked-Face-Dataset) and [Kaggle Face Mask Detection Dataset](https://www.kaggle.com/andrewmvd/face-mask-detection). 
2. Use [MTCNN](https://github.com/ipazc/mtcnn) to crop out faces for the images in the datasets (Labeled Faces in the Wild Dataset and Kaggle Face Mask Detection Dataset) and save them into a local directory. Split into training, validation, and testing portions.
3. Construct a neural network and train it on the training and validation datasets.
4. Evaluate the testing accuracy, precision, and F1 scores.
5. Construct a Mask Detection function: MTCNN to detect any input as images, use trained model weights to predict face/mask labels, spit out original image with boundary boxes and predicted labels.

## Integration with Instagram

Used [Sketch](https://www.sketch.com/) and an [Instagram Sketch Template](https://www.sketchappsources.com/free-source/2023-instagram-based-ui-kit-sketch-freebie-resource.html) to construct examples of how Instagram can potentially expand its platform using badges, mask donation incentives, and mask verification checks on photos.

## Tools

- Jupyter Notebook
- Google Cloud Compute Engine
- Google Colab
- Keras
- Tensorflow
- Numpy
- Sketch
