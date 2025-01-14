
# Neural Style Transfer with TensorFlow

This project implements Neural Style Transfer (NST) using TensorFlow and VGG19. It enables blending artistic styles with content images to create visually stunning outputs. The implementation includes advanced techniques like total variation loss, multi-layer feature extraction, and post-processing for enhanced image quality.

---

## Features
- **Style Transfer**: Combines the style of one image with the content of another using VGG19 layers.
- **Custom Initialization**: Supports initializing the generated image with random noise, content, or a blended mix of content and style.
- **Loss Functions**: Includes content loss, style loss, and total variation loss for improved visual coherence.
- **Post-Processing**: Sharpens, brightens, and enhances the resolution of the generated image.
- **Customizability**: Adjustable weights for style and content, as well as other hyperparameters.

---

## Requirements
- Python 3.7+
- TensorFlow 2.0+
- OpenCV
- NumPy
- Matplotlib

Install dependencies with:
```bash
pip install tensorflow opencv-python-headless numpy matplotlib

```

* * * * *

Usage
-----

### 1\. Clone the Repository

```
git clone https://github.com/yourusername/neural-style-transfer.git
cd neural-style-transfer

```

### 2\. Run the Script

Prepare your content and style images in the `images` directory. Then, execute the script:

```
python main.py

```

### 3\. Adjust Parameters

Modify the script to:

-   Change the weights for style and content loss.
-   Use different VGG19 layers for feature extraction.
-   Experiment with custom post-processing.

* * * * *

Project Structure
-----------------

```
.
├── images/
│   ├── content.jpg           # Input content image
│   ├── style.jpg             # Input style image
│   └── output/               # Directory for generated images
├── main.py                   # Main script for NST
├── utils.py                  # Utility functions for processing and enhancement
├── requirements.txt          # Python dependencies
└── README.md                 # Project documentation

```

* * * * *

Results
-------

Below are sample outputs from the project:

| Content Image | Style Image | Generated Image |
| --- | --- | --- |
| ![Content](https://chatgpt.com/c/images/content.jpg) | ![Style](https://chatgpt.com/c/images/style.jpg) | ![Generated](https://chatgpt.com/c/images/output/generated.jpg) |

* * * * *

How It Works
------------

1.  **Feature Extraction**: Uses pre-trained VGG19 layers to extract content and style features.
2.  **Optimization**: Minimizes a total loss combining content, style, and total variation losses.
3.  **Post-Processing**: Enhances the final output for sharpness, brightness, and resolution.

* * * * *

References
----------

-   [Original NST Paper by Gatys et al.](https://www.cv-foundation.org/openaccess/content_cvpr_2016/papers/Gatys_Image_Style_Transfer_CVPR_2016_paper.pdf)
-   TensorFlow VGG19 model

* * * * *

License
-------

This project is licensed under the MIT License. See `LICENSE` for details.

* * * * *

Acknowledgments
---------------

-   Thanks to TensorFlow and OpenCV communities for their excellent libraries.
-   Inspired by the PyTorch implementation of NST.

* * * * *

Happy creating! 🎨