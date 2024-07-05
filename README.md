Sure, here's the README content in a format you can directly copy to your GitHub repository:

---

# ImageC

## Overview

ImageC is a C++ project developed in collaboration with three students from the University of Porto, FEUP. The primary goal of the project is to convert PNG images into a two-dimensional matrix of pixels and provide various functionalities to manipulate these images.

## Features

- Convert PNG images to a pixel matrix
- Object-oriented design with three main classes: `Color`, `Image`, and `Script`
- A variety of image manipulation functionalities including:
  - Open image
  - Create blank image
  - Save image
  - Invert image colors
  - Convert image to grayscale
  - Replace a specific pixel
  - Fill the image
  - Mirror image (horizontally or vertically)
  - Add two images together
  - Crop image
  - Rotate image (left or right)
  - Apply median filter

## Classes

### Color

Represents a color with red, green, and blue components. Each component can be manipulated with values ranging from 0 to 255.

**Attributes:**
- `Red`
- `Green`
- `Blue`

### Image

Creates a two-dimensional matrix of colors (pixels) based on specified width and height. Each color corresponds to a pixel in the image.

**Methods:**
- Constructor to initialize the image with width and height
- Methods to access and manipulate individual pixels

### Script

Provides various functionalities to manipulate the image.

**Functionalities:**
- **Open Image:** Load an image from a file
- **Blank Image:** Create a blank image with specified dimensions
- **Save Image:** Save the current state of the image to a file
- **Invert Image:** Invert the colors of the image
- **Convert to Grayscale:** Convert the image to grayscale
- **Replace Pixel:** Replace a specific pixel with a new color
- **Fill Image:** Fill the entire image with a specific color
- **Mirror Image:** Mirror the image horizontally or vertically
- **Add Images:** Add two images together
- **Crop Image:** Crop the image to specified dimensions
- **Rotate Image:** Rotate the image left or right
- **Apply Median Filter:** Apply a median filter to the image

## Getting Started

### Prerequisites

- C++ compiler
- CMake (for building the project)
- PNG library (such as libpng) for handling PNG files

### Building the Project

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/ImageC.git
   ```
2. Navigate to the project directory:
   ```sh
   cd ImageC
   ```
3. Create a build directory:
   ```sh
   mkdir build
   cd build
   ```
4. Run CMake to configure the project:
   ```sh
   cmake ..
   ```
5. Build the project:
   ```sh
   make
   ```

### Usage

After building the project, you can use the executable to perform various image manipulations. Below is an example of how to use the `Script` class to manipulate an image:

```cpp
#include "Script.h"

int main() {
    Script script;

    // Open an image
    script.openImage("path/to/image.png");

    // Apply various operations
    script.invertImage();
    script.convertToGrayscale();
    script.mirrorImage(true); // true for horizontal, false for vertical
    script.saveImage("path/to/output.png");

    return 0;
}
```

## Authors
Leonardo Garcia - https://github.com/leonardorsg
Marcel Medeiros - https://github.com/marcelmedeiros1
Manoela Blanke - https://github.com/manoelablanke4

