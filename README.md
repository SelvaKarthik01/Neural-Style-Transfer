# Art Generation with Neural Style Transfer

This project implements **Neural Style Transfer (NST)** to create
artwork by blending the *content* of one image with the *style* of
another. The complete workflow is provided in the Jupyter Notebook:

    Art_Generation_with_Neural_Style_Transfer.ipynb

## Overview

Neural Style Transfer uses a pretrained **VGG19** model to extract:

-   Content features from the content image
-   Style features from the style image

A new image is then optimized to minimize content loss, style loss, and
total variation loss, resulting in a stylized output.

## Features

-   Load and preprocess content/style images
-   Extract feature maps from VGG19
-   Compute Gram matrices for style representation
-   Optimize the generated image using gradient descent
-   Produce high-quality artistic renderings

## Requirements

Install dependencies:

``` bash
pip install tensorflow pillow numpy matplotlib
```

## How to Run

1.  Open the notebook:

    ``` bash
    jupyter notebook Art_Generation_with_Neural_Style_Transfer.ipynb
    ```

2.  Update paths for:

    -   Content image
    -   Style image

3.  Run all cells to generate the stylized output.

## Folder Structure (example)

    /
    ├── Art_Generation_with_Neural_Style_Transfer.ipynb
    ├── content.jpg
    ├── style.jpg
    └── output/

## Customization

You can adjust:

-   `content_weight` → more structure
-   `style_weight` → more artistic texture
-   `total_variation_weight` → smoothness
-   Image size for higher resolution

## Future Enhancements

-   Multi-style blending
-   Real-time style transfer
-   Video style transfer
-   Web interface
