# Pneumonia Classification using Chest X-Ray Images

This project is a Pneumonia Classification system that uses a deep learning model to classify chest X-ray images into Pneumonia and Normal categories. The model is built using TensorFlow and Keras and can be deployed on the web using TensorFlow.js.

## Project Overview

The project consists of the following key components:
- **Model Training**: The deep learning model is trained using a dataset of chest X-ray images.
- **Model Conversion**: The trained TensorFlow model is converted to TensorFlow.js format for deployment on the web.
- **Web Deployment**: A simple web interface is provided for users to upload chest X-ray images and receive predictions on whether the image shows signs of pneumonia.

## Features

- **Deep Learning Model**: The model is based on Convolutional Neural Networks (CNN) and is trained on labeled chest X-ray images.
- **Web Interface**: A user-friendly web interface allows users to upload images and receive real-time predictions.
- **Deployment with TensorFlow.js**: The model is deployed using TensorFlow.js, allowing it to run directly in the browser without requiring a server.

## Installation

To get started with this project, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/sebukpor/pnemonia-detction-model.git
   cd your-repository-name
   ```

2. **Install dependencies**:
   Ensure you have TensorFlow and TensorFlow.js installed. If you haven't already, you can install them using:
   ```bash
   pip install tensorflow
   npm install @tensorflow/tfjs
   ```

3. **Convert the model to TensorFlow.js format**:
   If not already done, convert your trained model to TensorFlow.js format using:
   ```bash
   tensorflowjs_converter --input_format=tf_saved_model --output_format=tfjs_graph_model /path/to/saved_model /path/to/output_folder
   ```

4. **Upload the model files to GitHub**:
   Upload the `model.json` and weight files into the `model` folder in your GitHub repository.

5. **Deploy the Web Interface**:
   - Edit the `index.html` file provided in this repository to customize your web interface if necessary.
   - Ensure the paths in the `index.html` correctly point to the `model.json` and weight files in the `model` folder.

## Usage

To use the Pneumonia Detection system:

1. **Access the Web Interface**: Open the `index.html` file in your browser or host it on a web server.
2. **Upload an Image**: Use the upload button to select a chest X-ray image.
3. **Receive Prediction**: The model will process the image and display whether the image indicates pneumonia or not.

## Folder Structure

```plaintext
pneumonia-detection-model/
├── model/
│   ├── model.json
│   ├── group1-shard1of1.bin
│   └── ...
├── index.html
└── README.md
```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or suggestions, please contact the project maintainer at dasmedhub@gmail.com
