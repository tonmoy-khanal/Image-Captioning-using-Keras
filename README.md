# Teaching Computers to Describe Pictures

## Image Captioning

Image Captioning is the process of generating textual descriptions of an image. It uses both Natural Language Processing and Computer Vision to generate captions.

## Table of Contents

1. Introduction
2. Motive
3. Prerequisites
4. Data Collection
5. Interpreting Data
6. Data Cleaning
7. Loading the Training Set
8. Data Preprocessing — Images
9. Data Preprocessing — Captions
10. Data Preparation using Generator Function
11. Word Embeddings
12. Model Architecture
13. Inference
14. Evaluation
15. Conclusion and Future Work
16. References

## 1 - Introduction

### What is in this image?

![Image](https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Ftse2.mm.bing.net%2Fth%3Fid%3DOIP.BPMGsi39UsNLDf7-qBZwmwHaC7%26pid%3DApi&f=1)

Have you ever wondered how easy it is for humans to look at a picture and describe it in an appropriate language? Even a 5-year-old can do this with ease. However, the same task is challenging for computers.

### Problem Statement

Can you write a computer program that takes an image as input and produces a relevant caption as output for the given image? With the advent of Deep Learning, this problem can be solved with the right dataset.

Andrej Karapathy, who is now the Director of AI at Tesla, extensively researched this problem in his PhD thesis at Stanford.

### AIM

The aim is to explain, in simple terms, how Deep Learning can be used to solve the problem of generating a caption for a given image, hence the name **Image Captioning**.

**Caption Bot**: A state-of-the-art system created by Microsoft.

## 2 - Motive

Image captioning has several practical applications:

- **Image tagging for e-commerce, Photo-Sharing Services, and Online Catalogs.**
- **Automatic image annotations for blind individuals.**
- **CCTV Cameras**: With the prevalence of CCTV cameras, they can be used not only for monitoring but also for generating relevant captions. This can help in raising alarms in real-time for malicious activities in places such as malls or roads.
- **Automatic Captioning**: Imagine an Image Search as good as Google Search, where every image is first converted into a caption, and then a search can be performed based on the caption.

## 3 - Prerequisites

Before diving into image captioning, it's essential to understand the following Deep Learning concepts:

- Multi-layered Perceptrons
- Convolution Neural Networks (CNN)
- Recurrent Neural Networks (RNN)
- Transfer Learning
- Gradient Descent
- Backpropagation
- Overfitting
- Probability
- Text Processing
- Python (syntax and data structures)
- Keras library

### Encoder and Decoder

The image captioning process involves an **Encoder**, which is a Convolutional Neural Network (CNN) that extracts features from input images. The last hidden state of the CNN is connected to the **Decoder**, which is a Recurrent Neural Network (RNN) responsible for language modeling up to the word level.

[Understanding Encoder and Decoder](https://towardsdatascience.com/understanding-encoder-decoder-sequence-to-sequence-model-679e04af4346)

## 4 - Data Collection

There are numerous open-source datasets available for image captioning, such as:

- Flickr_8k_dataset (containing 8k images)
- Flickr_30k_dataset (containing 30k images)
- MS_COCO_dataset (containing 180k images)

For this project, we will use the Flickr_8k_dataset.

### AIM

The aim is to explain, in simple terms, how Deep Learning can be used to solve the problem of generating a caption for a given image, hence the name **Image Captioning**.

## 5 - Interpreting Data

The dataset consists of approximately 8,000 images, with each image having five captions. Each image-caption pair is relevant. The dataset is divided into the following parts:

- **Test Set**: 1,000 images
- **Training Set**: 6,000 images
- **Dev Set**: 1,000 images

The dataset is in the form of [image → captions], where the images are accompanied by corresponding output captions. These captions are crucial for training the image captioning model.

### Dataset Structure

The dataset structure consists of images and corresponding captions. The `captions.txt` file contains the names of each image along with its five captions (0-4).

[Download Dataset](https://forms.illinois.edu/sec/1713398)

## 6 - Data Cleaning

Data cleaning involves tasks like removing duplicates, handling missing values, and ensuring consistency in the data. It is essential to prepare the data for further processing and training.

## 7 - Loading the Training Set

To train an image captioning model, we need to load the training set, which consists of 6,000 images along with their relevant captions.

## 8 - Data Preprocessing — Images

Preprocessing images includes tasks like resizing, normalizing, and extracting features using a pre-trained CNN. These features are crucial for the image captioning model.

## 9 - Data Preprocessing — Captions

Caption preprocessing involves tasks like tokenization, padding, and preparing captions for training.

## 10 - Data Preparation using Generator Function

Data preparation is a crucial step in training an image captioning model. A generator function is used to create batches of data for training and validation.

## 11 - Word Embeddings

Word embeddings are used to represent words in a format that can be understood by the model. These embeddings are essential for the language model in the image captioning process.

## 12 - Model Architecture

The model architecture for image captioning includes both the encoder and decoder. It combines Computer Vision and Natural Language Processing to generate captions for images.

## 13 - Inference

Inference involves using the trained model to generate captions for new images. It showcases the practical application of image captioning.

## 14 - Evaluation

Evaluating the performance of the image captioning model is essential to ensure that the generated captions are relevant and accurate.

## 15 - Conclusion and Future Work

The conclusion summarizes the key findings of the project, and future work discusses potential improvements and extensions of the image captioning model.

## 16 - References

References provide citations and sources for the research and resources used in the project.
