# Using Raspberry Pi to calculate the refraction index for liquids by image processing techniques.

In this project, I employed the Raspberry Pi camera module to capture images, enabling the application of advanced image processing techniques using Python. 

The objective of the project was to determine the refraction index of liquids by leveraging image analysis methodologies.

The image processing pipeline has several essential steps, including the conversion of captured images to grayscale to facilitate subsequent analysis. 
Afterwards, certain areas that we wanted to focus on were intentionally made black in order to reduce any factors that could cause problems, like being too bright or having reflections.
An then a thresholding technique was applied to segment the image based on intensity levels, resulting in a binary representation.

Utilizing the binary image, the coordinates of relevant features were extracted using numpy. These coordinates were subsequently utilized to calculate the refraction index based on established mathematical formulations. Notably, the calculations took into account the distances between the detected coordinates, enabling the estimation of the refraction index for the analyzed liquid samples.

I provided codes as well in this repository.

It's still a good practice to perform additional testing and validation to ensure the code's reliability across a wider range of scenarios or input variations.


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


