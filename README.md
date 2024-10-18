# dl_self-driving_car
Here lies the first version of the miniature self driving car with deep learning.

Hardware components:
1. Raspberry Pi 4 Model B
2. Google's Edge TPU

Hardware knowledge requirements:
- ??
- ??

Software knowledge requirements:
- Single shot multi-box object detection
- Transfer learning

Outline:
1. We start with the brain of our car, the raspberry pi
    1.1 Setup Raspbian OS on microcontroller
    1.2 Setup remote access via SSH and VNC (so a gui can pop up on your PC)
    1.3 Setup Samb File Server on RPI 
    1.4 Connect to the pi computer from PC

2. Next with just the RPI, we test camera input to ensure it works
    2.1 Install a video camera viewer (cheese) in the raspberry pi terminal
    2.2 Run cheese

3. Setup car body with all the motors, wires, 
    3.1 ???
    3.2 ???
    3.3 ???

4. At this point, the car is able to move and display video with python commands, but now we test the image processing
    4.1 Install OpenCV and related libraries that OpenCV uses
    4.2 Test OpenCV installation, checking if the folder "cv2" exists
    4.3 Do live video processing with OpenCV, converting original image input to B&W to ensure library works

5. Now we need to install ***TensorFlow*** for the RPI CPU and EdgeTPU, where the CPU runs ***inference***  (based on a pretrained model), while the TPU runs deep learning
    5.1 Install tensorflow and ***keras*** with pip3 for the cpu
    5.2 For what models work on the TPU, refer to: https://coral.ai/docs/edgetpu/models-intro/
    5.3 




*** inference means model prediction, or in other words, only forward propagation
*** keras is a library that makes building ml models easy. you can build models with easy calls, do various things like data preprocessing, training, fine-tuning, model evaluation, and tensorflow functionality.
*** TensorFlow is a full-fledged machine learning framework used to build, train, and deploy ml models at a lower level (like down to the math). TF is designed for scale, and does automatic differentiation/optimization, and allows graph based computation (whatever that means). It's supported on Python, Java, C++, JavaScript


Future work:
Better object detection models: https://medium.com/tech-spectrum/top-10-object-detection-models-in-2024-7dc3f830e9dd






