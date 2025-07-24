# MRXS to Cropped PNG Converter

This Python script converts digital pathology MRXS files to high-resolution PNG images.  
It automatically detects and crops the region of interest (ROI), removing black space around the tissue.  
Progress bars and detailed timing statistics are provided for profiling and monitoring.

## Features

- Detects the main image region (ROI) at low resolution, for efficiency
- Crops and exports the ROI at original (highest) resolution
- Saves as PNG (lossless, suitable for medical/scientific use)
- Provides detailed timing information for each stage
- Interactive progress bars via `tqdm`
- Error handling with clear feedback

## Requirements

- Python 3.7+
- OpenSlide Python bindings
- OpenSlide (native library)
- Pillow (PIL)
- numpy
- opencv-python
- tqdm

Install dependencies via pip:

```bash
pip install -r requirements.txt

