 # Neural Style Transfer Using TensorFlow  

This project demonstrates **Neural Style Transfer**, where one image's content is combined with another's artistic style to create a visually appealing artwork. The implementation uses TensorFlow and the pre-trained VGG19 model to extract content and style features for the transfer.  

## Table of Contents  
1. [Overview](#overview)  
2. [Features](#features)  
3. [Dataset](#dataset)  
4. [Installation](#installation)  
5. [Usage](#usage)  
6. [Results](#results)  
7. [License](#license)  

---

## Overview  
Neural Style Transfer leverages deep learning to apply the artistic style of a painting to the content of a different image. This project allows users to:  
- Load and preprocess input images.  
- Use a pre-trained **VGG19 model** to extract content and style representations.  
- Optimize a generated image to blend the content and style.  

---

## Features  
- Combines content and style using deep learning.  
- Supports high-quality images for realistic and artistic outputs.  
- Configurable hyperparameters (learning rate, iterations, etc.).  

---

## Dataset  
The dataset used for this project is the [Images for Style Transfer Dataset](https://www.kaggle.com/soumikrakshit/images-for-style-transfer).  

It contains two main folders:  
- **Artworks**: Artistic paintings for style reference.  
- **TestCases**: Photographs for content reference.  

---

## Installation  
1. Clone this repository:  
   ```bash  
   git clone https://github.com/YourUsername/Neural-Style-Transfer.git  
   cd Neural-Style-Transfer  
   ```  

2. Install dependencies:  
   ```bash  
   pip install tensorflow tensorflow-addons numpy pillow kagglehub  
   ```  

3. Download the dataset using KaggleHub:  
   ```python  
   import kagglehub  
   kagglehub.dataset_download("soumikrakshit/images-for-style-transfer")  
   ```  

---

## Usage  
### Running the Style Transfer:  
1. Place the **content image** and **style image** paths in the code.  
2. Run the Jupyter notebook or Python script to generate the stylized image.  
3. The output image is saved as `stylized_image.jpg`.  

### Key Hyperparameters:  
- **num_iterations**: Number of optimization iterations.  
- **learning_rate**: Learning rate for the Adam optimizer.  

---

## Results  
Below is an example of the output:  

| Content Image | Style Image | Stylized Output |  
|---------------|-------------|-----------------|  
| ![Content](path/to/content_image.jpg) | ![Style](path/to/style_image.jpg) | ![Stylized](path/to/stylized_image.jpg) |  

Feel free to replace with your generated results!  

---

## License  
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.  
