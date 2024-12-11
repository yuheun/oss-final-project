# **Face Blur Detection with OpenCV**
### Automatically detects and blurs faces in images using OpenCV

This project implements a simple Python program to detect faces in images and apply a blur effect to preserve privacy. The solution leverages OpenCV's Haar Cascade classifier for face detection and Gaussian blur for obfuscating the detected faces.

---

## **Key Points**
1. **Steps involved**:
    1. Load the input image.
    2. Convert the image to grayscale for faster processing.
    3. Use Haar Cascade to detect faces in the image.
    4. Extract the regions of interest (ROIs) corresponding to the detected faces.
    5. Apply Gaussian blur to the ROIs.
    6. Replace the original face regions with the blurred ones.
    7. Save and display the processed image.
2. **Assumptions**:
    - The image contains at least one face.
    - The Haar Cascade model is pre-trained and included in the OpenCV library.
3. **Practical Use Cases**:
    - Masking faces in public surveillance footage.
    - Anonymizing faces in social media photos or research datasets.

---

## **Requirements**
1. Python (3.7+)
2. OpenCV (4.1.0 or higher)
3. Numpy (1.16.4 or higher)

---

## **Commands to run the face blur program**
```bash
python face_blur.py --image images/input.jpg --output images/output.jpg
```

## **Results:**
This implementation is effective at detecting faces and applying a blur effect. Below is an example of the input and output:

![JPG of input image](images/input.jpg)
![JPG of ouput image(Blurred Faces)](images/output.jpg)


## **The limitations**
This technique relies on Haar Cascade's face detection accuracy, which may fail in poor lighting or with occluded faces.
Gaussian blur is a basic obfuscation technique. For sensitive applications, encryption or advanced anonymization might be needed.