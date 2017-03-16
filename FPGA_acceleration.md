## Acclerator Edge Detection in FPGA

![alt tag](https://cloud.githubusercontent.com/assets/17951883/23996071/2b1df750-0a72-11e7-97fe-08915c0668e1.png)


## Steps to reduce bandwidth in FPGA accleration module for Sobel Filter

-> as original pixels once read is used to compute three derivative pixels in each kernel convolution same and preceding columns , So rather than re-reading we can store it in our accelerator for use in computing multiple derivative pixels.< br/>

->we could design small pixels in our accelerator to store complete rows read from the sensor.This would allow each pixel to be read only n=once.
