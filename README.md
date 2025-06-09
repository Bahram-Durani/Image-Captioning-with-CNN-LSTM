### Image Captioning with CNN + LSTM

This project implements an image captioning system using a combination of Convolutional Neural Networks (CNNs) and Long Short-Term Memory (LSTM) networks. It uses the **Flickr8k** dataset for training and evaluation.

---

### Technologies & Frameworks Used

- **Python 3.x**
- **TensorFlow/Keras** – Deep learning framework
- **Xception Model** – Pretrained CNN model used as feature extractor
- **LSTM** – Recurrent Neural Network for generating captions
- **Tokenizer** – For text preprocessing and sequence generation
- **tqdm** – Progress bar for loops
- **PIL / NumPy / Matplotlib** – Data manipulation and visualization
- **tf.data.Dataset** – Efficient data loading and batching

---

###  Dataset Used

This project uses the **Flickr8k** dataset:

1. **Flickr8k_Dataset**: Contains the images.
2. **Flickr8k_text**: Contains image captions.

Dataset Link: https://www.kaggle.com/datasets/adityajn105/flickr8k 

### Model Architecture

#### The model consists of two parts:

1. CNN Encoder:

   * Uses Xception (pretrained on ImageNet) to extract 2048-dimension features from images.
  * These are further compressed into a 256-dimension vector.

2. LSTM Decoder:

* An LSTM layer that takes both the image features and previously generated words to predict the next word in the caption.

  ### Model Diagram

  ![image](https://github.com/user-attachments/assets/428ad0a8-ea90-4cd9-989e-1c58a4018d6d)

