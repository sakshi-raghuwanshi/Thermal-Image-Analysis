# Thermal Image Analysis
A tool for analyzing and annotating thermal images.

This repo relies on the [thermal_base python package](https://github.com/detecttechnologies/thermal_base) for image decoding and manipulation backend.

[![Quality check](https://github.com/detecttechnologies/Thermal_Image_Analysis/actions/workflows/qualitycheck.yml/badge.svg)](https://github.com/detecttechnologies/Thermal_Image_Analysis/actions)

## Features
# sakshi 
<p align="center"><img src="assets/images/main.gif" /><br/>Main menu</p>

### Spot marking, line measurement and area marking

- Extract the temperature values at marked spots
- Plot temperature values along the marked line(s)
- Get min, max and average values of marked regions

Generates a plot for line plots and a table for measurements in the marked regions.

<p align="center"><img src="assets/images/markings.png" /><br/>Markings on the image.</p>

<p align="center">
    <img src="assets/images/graph.png" width="50%"/>
    <img src="assets/images/table.png" width ="49%"/>
    <br/>Plots and measurements.
</p>


### ROI scaling
Scale the entire image based on values in the marked region. Use to enhance low contrast areas.

<p align="center"><img src="assets/images/roi.png" /><br/>ROI scaling interface.</p>

### Change colormap
Change colormap to one of the following options:

<p align="center"><img src="assets/images/cmap.gif" /><br/>Change colormap.</p>

### Emissivity scaling
Change reflected apparent temperature and emissivity of marked region.

<p align="center"><img src="assets/images/emm.png" /><br/>Emissivity scaling interface.</p>

### Save data
Image can be saved with or without markings, plots and values. Custom savefile(.pkl) saves all data and can be used to revive the previous session. New supported save extensions are :
 - CSV : Saves thermal values of a thermal image in Kelvin as a CSV format.
 - TIFF: Saves thermal values of a thermal image in Kelvin as a TIFF format.

<p align="center"><img src="assets/images/saveProcess.gif" /><br/>Saving process.</p>

## Installation
 - Run installation once with `pip install -r requirements.txt`
 - Install [exiftool](https://exiftool.org/install.html)

## Usage
 - Run the program with `python main.py`
 - Select the original thermal image file or the custom saved `.pkl` file. (Find some samples in `sample_images`)
 
