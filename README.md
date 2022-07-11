# Bare-PCB-defect-detection-using-OpenCV

This project implements the detection of bare PCB defects such as missing hole, mouse bite and open circuit, using the OpenCV library in Python. 
<br> The image processing technique called Image Subtraction is used for the purpose of defect detection.

The Bare-PCB-images-dataset folder contains the dataset used for this project, and its details in a README file. It contains RGB images of five types of bare PCBs. It includes both the non-defective and defective PCB images.

Example of bare PCB having missing hole defect:

![Annotated PCB image with missing hole defect](https://user-images.githubusercontent.com/59477814/130058005-02531758-5d4f-47f9-bd61-749155690dab.png)


The Jupyter notebook has the code for the step-by-step PCB defect detection process using image subtraction. The steps, which apply to both template and test images, involve converting the original image to grayscale, applying Gaussian blur to blur the image and then using adaptive thresholding to convert the image to a binary image. 
<br> Once both the images are binary, the test image is subtracted from template to get the resultant image (difference image) which shows the defects. 
<br> Contour detection is then used to get the number of defects in the final image.

An example of a final result image showing defects looks like this:

![Resultant binary image](https://user-images.githubusercontent.com/59477814/130059689-0ed9bc9d-9b32-4961-bb89-cca6d2984a2d.png)
