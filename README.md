#ImageProcessor
A modular Python script for performing common image processing tasks using OpenCV, including loading images, adjusting brightness and contrast, blurring, denoising, edge detection, and feature extraction using SIFT.

#📦 Features
-✅ Load images with format validation

-✅ Adjust brightness and contrast

-✅ Apply Gaussian blur

-✅ Apply Non-local Means Denoising

-✅ Perform Canny edge detection

-✅ Extract features using SIFT descriptors

-✅ Save processed images to disk

#🛠 Requirements
Python 3.6+

OpenCV (cv2)

NumPy

Install the required packages using:


pip install opencv-python numpy
For SIFT to work, you may need the opencv-contrib-python package:


pip install opencv-contrib-python
#🚀 Usage
Run the Script
Place your image in a known directory and edit the path in the main() function:


input_path = "/content/images (1).jpeg"
Then run the script:


python image_processor.py
Output
The script processes the image and saves:

Brightness/contrast adjusted image

Gaussian blurred image

Denoised image

Canny edge map

Each image is saved using the original filename with a suffix (e.g., image_adjusted.jpg).

#🧩 Class Overview
ImageProcessor
Method	Description
load_image(path)	Loads and validates an image
adjust_brightness_contrast	Modifies brightness and contrast of the image
apply_gaussian_blur	Applies Gaussian blur
apply_denoising	Removes noise using Non-local Means Denoising
apply_canny_edge	Detects edges using Canny method
extract_features	Extracts SIFT features from the image
save_image	Saves the image to a specified path

#📂 Example Output Files
-images (1)_adjusted.jpg

-images (1)_blurred.jpg

-images (1)_denoised.jpg

-images (1)_edges.jpg

#📃 License
This project is open source and free to use for educational and personal projects.
