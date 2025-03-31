# create-photo-slideshow
## Images to PowerPoint Presentation  A Python script to automatically generate a PowerPoint (.pptx) presentation from a folder of images. Each image is placed on its own slide, scaled to fit maximally while preserving aspect ratio, and centered. Uses `python-pptx` and `Pillow`.

# Auto Image-to-PowerPoint Slideshow Generator

This repository contains a Python script designed to streamline the process of creating PowerPoint presentations directly from a directory of images. Instead of manually inserting, resizing, and centering each image onto slides, this script handles it automatically.

## Problem Solved

Creating image-heavy presentations often involves repetitive tasks: adding a new slide, inserting an image, resizing it to fit the slide nicely without distortion, and centering it. This script automates this entire workflow.

## How it Works

The script iterates through image files (common formats like PNG, JPG, GIF, etc.) found within a specified input folder (`images` by default). For each image, it:

1.  Adds a new blank slide to a PowerPoint presentation.
2.  Calculates the optimal dimensions to scale the image so it fills as much of the slide as possible without exceeding the slide boundaries or distorting the original aspect ratio.
3.  Determines the correct positioning to center the scaled image on the slide.
4.  Inserts the image onto the slide with the calculated size and position.
5.  Saves the final result as a `.pptx` file, ready to be opened in Microsoft PowerPoint.

## Requirements

* Python 3
* `python-pptx` library: `pip install python-pptx`
* `Pillow` library: `pip install Pillow`

## Getting Started

1.  Clone or download this repository.
2.  Ensure you have Python and the required libraries installed.
3.  Create a folder named `images` in the same directory as the script.
4.  Populate the `images` folder with the pictures you want in your presentation.
5.  Run the script from your terminal: `python your_script_name.py`
6.  A `.pptx` file (e.g., `MyImagePresentation.pptx`) will be generated in the same directory.