🔍 Project Overview

This project implements an Image Caption Generator using an LSTM-based model, which combines computer vision (via CNNs) with natural language processing to generate textual descriptions for images.

📌 Key Features

CNN Feature Extraction: Uses a pre-trained InceptionV3 model to extract features from images.

LSTM Decoder: Takes image features + partial captions to predict the next word.

Tokenizer & Padding: Processes captions and ensures consistent input size.

Greedy Search: Generates captions word-by-word from the trained model.

🚀 How to Run
Preprocess Data

Format captions.

Extract image features using InceptionV3.

Train the Model

Use ImageDataGenerator and the prepared sequences to train the model.

Generate Captions

Load a test image.

Use greedy search to predict the caption.

🧠 Model Architecture
Encoder: InceptionV3 (pre-trained, removes final layer).

Decoder:

Embedding Layer

LSTM (256 units)

Dense layers for output vocabulary

🧪 Evaluation
The model uses BLEU score for evaluation of caption quality.

📸 Example Output

<img width="275" height="183" alt="image" src="https://github.com/user-attachments/assets/9f10bd89-304f-4167-8377-91648cfc47c3" />

"a dog is running in the field"
