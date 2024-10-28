# Color Detection App

A Python-based Color Detection App that identifies the color name of a pixel in an image upon double-clicking. This project uses OpenCV and Pandas to detect color names from a CSV file containing color data.

## Table of Contents
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [CSV File Format](#csv-file-format)

## Features
- **Detect RGB Values**: Displays the RGB values of the pixel you click on.
- **Display Color Names**: Shows the name of the color closest to the clicked pixel based on a dataset.
- **Light and Dark Color Handling**: Adjusts text color for visibility based on light or dark background.

## Installation

### Prerequisites
- Python 3.x
- OpenCV
- Pandas
- Numpy

### Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/AadityaPanda/Image-Colour-Identifier.git
   ```
2. Install the required packages:
   ```bash
   pip install opencv-python-headless pandas numpy
   ```

3. Ensure you have a `colors.csv` file in the same directory as the script. A sample CSV format is explained below.

## Usage
Run the script from the command line and pass an image file path as an argument:

```bash
python color_detection.py -i path_to_image.jpg
```

### How to Use
1. Launch the script with the image path.
2. Double-click on any pixel in the image window to see its color name and RGB values.
3. Press the **ESC** key to exit the application.

## Project Structure
```
Image-Colour-Identifier/
├── colors.csv               # CSV file with color names and RGB values
├── color_detection.py        # Main Python script for the color detection app
└── README.md                 # Project README
```

## CSV File Format
The `colors.csv` file should have the following columns:
- **color**: Index or ID of the color.
- **color_name**: Name of the color (e.g., Red, Blue).
- **hex**: Hexadecimal code of the color (e.g., #FFFFFF for white).
- **R**: Red component (0-255).
- **G**: Green component (0-255).
- **B**: Blue component (0-255).

Example CSV Content:
```csv
color,color_name,hex,R,G,B
0,Black,#000000,0,0,0
1,White,#FFFFFF,255,255,255
2,Red,#FF0000,255,0,0
...
```
