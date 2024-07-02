# Face Mask Detection Project
## Overview
This project utilizes a YOLOv8l model trained for detecting face masks in images. The model classifies images into three categories: wearing mask correctly, not wearing mask, and not wearing mask properly. It aims to provide a solution for monitoring adherence to face mask guidelines in public spaces.

## Dataset and Annotations
The dataset used for training and validation is sourced from Kaggle's  [Face Mask Detection dataset](https://www.kaggle.com/datasets/andrewmvd/face-mask-detection "Face Mask Detection dataset"). The dataset consists of images annotated with bounding boxes specifying regions of interest (ROI) around faces with different mask categories.

## Data Preprocessing
* **XML Parsing:** XML annotations are parsed to extract image names and instance details.
* **Dataset Structuring:** Images are organized into YOLOv8-compatible folder structures (`dataset/images/train, dataset/images/validation`) along with corresponding label files (`dataset/labels/train, dataset/labels/validation`).

## Model Architecture
The YOLOv8l model from Ultralytics is utilized for its efficient object detection capabilities. Instead of training from scratch, a pretrained model from [Kaggle's model repository](https://www.kaggle.com/models/shivam2111/yolov8l-mask-detection/PyTorch/yolov8l-v1.0/1/ "Kaggle's model repository") is employed, which has been fine-tuned for face mask detection.

**To know more about fine tuning process you can look at [fine-tuning process](https://www.kaggle.com/code/shivam2111/face-mask-detection-yolov8l)**

## Installation and Setup
### Requirements
Ensure the following dependencies are installed:

* Python 3.x
* Required Python packages (listed in requirements.txt)

### Setup Instructions
1. Clone the repository:

```bash
git clone https://github.com/your-username/your-repository.git
cd your-repository
```

2. Install dependencies:

```bash
pip install -r requirements.txt
```
## Usage
You can run the notebook and all the necessary files will be created/downloaded.

## Example

[output.webM](https://github.com/Shivam-21-11/mask-detection-yolov8L/assets/66676220/a8048555-6fc1-42a4-9854-fd02120bbc35)


## Acknowledgements

* The dataset is sourced from Kaggle's [Face Mask Detection dataset](https://www.kaggle.com/datasets/andrewmvd/face-mask-detection "Face Mask Detection dataset").
* The YOLOv8 model is provided by [Ultralytics](https://docs.ultralytics.com/models/yolov8/ "Ultralytics").

## Contributing
Contributions are welcome! Please fork the repository and create a pull request with your improvements.

## License
MIT License

Copyright (c) 2024 Shivam Singh

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

