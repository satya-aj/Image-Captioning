## Image Captioning

Given an image, goal is to generate a caption fot that Image

### using Attention-based model

- Preprocess the images using InceptionV3
- Useing pretrained Imagenet Weights
- Features extraction from lower convolutional layer of InceptionV3 giving a vector shape of (8, 8, 2048)
- This vector then passed through CNN Encoder(FC layer)
- The RNN (GRU layer) attends over the image to predict the next word
- Preprocess and tokenize the captions
- Evaluate the image and get captions
