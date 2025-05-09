# SMS Spam Classifier 📱✉️

This project is a neural network built with TensorFlow and Keras to classify SMS messages as either "ham" (legitimate) or "spam" (unwanted promotional messages).

## 📊 Dataset
We use the [SMS Spam Collection Dataset](https://www.dt.fee.unicamp.br/~tiago/smsspamcollection/), already split into training and validation sets (`train-data.tsv` and `valid-data.tsv`).

## 🧠 Model Architecture

- **Text Vectorization** with TensorFlow's `TextVectorization` layer
- **Embedding Layer** to map words to vector space
- **Dense Layer (32 neurons, ReLU)** to learn patterns
- **Dropout Layer (0.2)** to prevent overfitting
- **Output Layer (1 neuron, Sigmoid)** for binary classification

## ⚙️ Training

- Optimizer: Adam  
- Loss: Binary Crossentropy  
- Epochs: 10  
- Batch Size: 32  
- Accuracy: ~97% on validation data

## 🧪 Prediction Function

A `predict_message()` function takes a string and returns a list:  
`[probability, 'ham' or 'spam']`

Example:
predict_message("You have won $1000! Call now!")  
# Output: [0.912, 'spam']

🚀 Getting Started
Clone the repo

Install dependencies: pip install tensorflow tensorflow-datasets

Run the notebook
