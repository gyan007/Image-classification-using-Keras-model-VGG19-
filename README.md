# Image-classification-using-Keras-model-VGG19


## Overview

The **Image Classifier** is a web-based application that uses a deep learning model to predict the category of an image. It is built with **Flask** for the backend and utilizes the **VGG19** pre-trained convolutional neural network (CNN) for image classification. The model is deployed in the application using **TensorFlow**. This project aims to provide an easy-to-use interface for users to upload images and get predictions about the image categories.

## Features

* Upload an image in formats such as `.png`, `.jpg`, or `.jpeg`.
* Displays the uploaded image for preview.
* Predicts the image category using the VGG19 model pre-trained on ImageNet data.
* Shows the predicted result with the image classification label.
* User-friendly web interface with intuitive design and smooth interactions.

## Tech Stack

* **Frontend**: HTML, CSS, JavaScript (Tailwind CSS for styling)
* **Backend**: Python, Flask
* **Model**: VGG19 (pre-trained on ImageNet)
* **Deep Learning Framework**: TensorFlow
* **Other Libraries**: Keras, werkzeug

## How It Works

1. The user uploads an image through a file input.
2. The image is sent to the Flask server using a POST request.
3. The Flask app processes the image and feeds it into the **VGG19** model, which has been pre-trained on the **ImageNet** dataset.
4. The model classifies the image and sends back the predicted label.
5. The frontend displays the predicted label along with the uploaded image.

## Installation

### Prerequisites

Make sure you have the following installed:

* Python 3.x
* pip (Python package manager)

### Setting Up the Project

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/image-classifier.git
   ```

2. Navigate to the project directory:

   ```bash
   cd image-classifier
   ```

3. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Download the pre-trained model (`vgg19.h5`) or train it using the provided script `model.ipynb` and save it as `vgg19.h5`.

5. Run the Flask application:

   ```bash
   python app.py
   ```

6. The application will run locally at `http://127.0.0.1:5000/`. Open this URL in your browser.

## Usage

1. Navigate to the home page of the application.
2. Click the **Choose...** button to upload an image file.
3. After the image is uploaded, click the **Predict!** button to get the predicted label for the image.
4. The predicted result will be displayed below the image.

## Folder Structure

```
image-classifier/
│
├── app.py                # Main Flask application file
├── untitled.ipynb           # Jupyter notebook for training and saving the model
├── vgg19.h5              # Pre-trained VGG19 model file
├── static/               # Folder for static assets (images, stylesheets, etc.)
│   └── css/              # Custom styles
│       └── style.css
│   └── js/              # Custom styles
│       └── main.js
├── templates/            # Folder for HTML templates
│   └── index.html        # Main template for the app
│   └── base.html         # Main template for the app
├── uploads/              # Folder to store uploaded images
```

## Dependencies

The project requires the following Python packages:

* Flask
* TensorFlow
* Keras
* werkzeug
* gevent

You can install the dependencies by running:

```bash
pip install -r requirements.txt
```

## Contributing

If you wish to contribute to this project, feel free to fork the repository and make your changes. Once you have made your modifications, please submit a pull request with a description of the changes.

## License

This project is open-source and available under the MIT License.

## Acknowledgements

* VGG19 model pre-trained on ImageNet.
* Flask for creating the web application.
* TensorFlow and Keras for providing the deep learning framework and pre-trained model.
* Tailwind CSS for styling the frontend.

---

You can customize the repository URL and any other project-specific details as needed!
