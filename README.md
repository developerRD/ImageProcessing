# Using Raspberry Pi to calculate the refraction index for liquids by image processing techniques.

In this project, I used the Raspberry Pi camera module to capture images, allowing for advanced image processing techniques in Python.

The goal of the project was to determine the refraction index of liquids by applying image analysis methods.

The image processing pipeline has several key steps, including converting the captured images to grayscale to make analysis easier. Afterwards, specific areas we wanted to focus on were intentionally blacked out to reduce issues like excessive brightness or reflections. Then, a thresholding technique was applied to separate parts of the image based on intensity levels, creating a binary version of the image.

Using the binary image, the coordinates of relevant features were extracted with numpy. These coordinates were then used to calculate the refraction index based on established mathematical formulas. Importantly, the calculations considered the distances between the detected coordinates, allowing an estimate of the refraction index for the liquid samples analyzed.

I’ve also provided the code for this project in the repository.

It’s a good practice to perform additional testing and validation to ensure the code works reliably across different scenarios and inputs.


<img width="430" alt="Screenshot 2023-06-22 at 3 17 35 PM" src="https://github.com/developerRD/ImageProcessing/assets/34951241/dd2a00a4-fa09-4c50-909b-f5df5168363e">

The first step involves activating the camera module, which captures real-time imagery. Concurrently, visual cues in the form of lines are superimposed on the camera feed, offering guidance on the precise positioning required to obtain accurate measurements. These lines serve as reference points for aligning the laser pointer and the liquid-filled glass cup within the camera frame.

<img width="481" alt="Screenshot 2023-06-22 at 3 18 41 PM" src="https://github.com/developerRD/ImageProcessing/assets/34951241/e72de86a-a7cc-4c53-95d8-10934be75bb0">

grayscale to facilitate subsequent analysis

<img width="541" alt="Screenshot 2023-06-22 at 3 19 18 PM" src="https://github.com/developerRD/ImageProcessing/assets/34951241/6254a3f7-85d9-4169-a90a-c63fa14cb364"> 

binary representation, black and white picture

<img width="433" alt="Screenshot 2023-06-22 at 3 20 32 PM" src="https://github.com/developerRD/ImageProcessing/assets/34951241/f648ea24-05ec-4dd2-b953-9fb316e22e42">

And this is the final picture that shows the results. 

English translated results are belove: 

Location of laser light : [30 504 ] 

Location of the laser pointed on surface : [207 301]

Position in the liquid after the light is refracted: [407 305]

Refraction: 1.284646

In this experiment, the refractive index was taken as the measured liquid water.
The refractive index of water is 1.33. The concluding value was 1.28 with a margin of error of 3.75%.


