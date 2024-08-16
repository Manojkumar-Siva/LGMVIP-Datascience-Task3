# LGMVIP-Datascience-Task3

# Image to Sketch with Python:
The objective of this exercise is to transform a color image into a visually appealing pencil sketch by leveraging image processing techniques. This process involves several key steps, each aimed at enhancing the visual characteristics of the sketch to resemble a hand-drawn artwork. 


## Algorithm:

### Step1: 
Read and Convert to RGB: Since OpenCV loads images in BGR format by default, we convert it to RGB for correct color representation.
### Step2: 
Convert to Grayscale: We convert the image to a grayscale format to reduce complexity and prepare it for further processing.
### Step3:
Invert the Grayscale Image: We use cv2.bitwise_not() to invert the pixel values, creating a negative image.
### Step4:
Blur the Inverted Image: Gaussian Blur is applied to smooth the image. This blurring simulates the soft texture of pencil strokes
### Step5:
Create the Pencil Sketch: The sketch effect is achieved by dividing the grayscale image by the blurred inverted image using cv2.divide(), which enhances the details and gives a pencil-like appearance.
