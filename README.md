# Using Raspberry Pi to calculate the refraction index for liquids by image processing techniques.

In this project, I captured an image using the Raspberry Pi camera, applied various image processing techniques with Python, and calculated the refraction index based on the detected coordinates.

I provided codes here in this repository.

It's still a good practice to perform additional testing and validation to ensure the code's reliability across a wider range of scenarios or input variations.


<img width="430" alt="Screenshot 2023-06-22 at 3 17 35 PM" src="https://github.com/developerRD/ImageProcessing/assets/34951241/dd2a00a4-fa09-4c50-909b-f5df5168363e">

When the codes run, first a camera starts running and you can see the lines on the camera that shows you how to take the picture in order to get the correct results.
In order to work with this code and measure the refractive index for liquids, you need a laser pointer and liquid in a glass cup that can be shown in the pictures.

<img width="481" alt="Screenshot 2023-06-22 at 3 18 41 PM" src="https://github.com/developerRD/ImageProcessing/assets/34951241/e72de86a-a7cc-4c53-95d8-10934be75bb0">

Gray scale of the picture for calculations

<img width="541" alt="Screenshot 2023-06-22 at 3 19 18 PM" src="https://github.com/developerRD/ImageProcessing/assets/34951241/6254a3f7-85d9-4169-a90a-c63fa14cb364"> 

Turned the picture into black and white, that way we can only work on 0 and 1 values for our calculations. 

<img width="433" alt="Screenshot 2023-06-22 at 3 20 32 PM" src="https://github.com/developerRD/ImageProcessing/assets/34951241/f648ea24-05ec-4dd2-b953-9fb316e22e42">

And this is the final picture that shows the results. 
Since my first language is Turkish, I completed this project in some parts of the Turkish language but here I Provided a translation for you.

Location of laser light : [30 504 ] 

Location of the laser pointed on surface : [207 301]

Position in the liquid after the light is refracted: [407 305]

Refraction: 1.284646

In this experiment, the refractive index was taken as the measured liquid water.
The refractive index of water is 1.33. As a result, the value we obtained was obtained as 1.28 with a margin of error of 3.75%.


