# SuperRes-RFF
## Title
**Advanced Image Enhancement and Data Recovery: Superresolution Techniques and Missing Data Handling**<br>

## Description
This project focuses on enhancing image resolution and reconstructing images with missing data using advanced machine learning techniques. Specifically, it applies superresolution to enhance image quality and employs `Random Fourier Features (RFF)` combined with `linear regression` for image reconstruction. The project involves both qualitative and quantitative analyses to evaluate the performance of these methods. Key tasks include `superresolution enhancement`, measuring reconstruction accuracy with various metrics, and handling images with different levels of missing data<br>

## Project Task
- **Superresolution Enhancement** : Performing Superresolution on the image to enhance its resolution by factor `2`. Displaying a qualitative comparison of original and reconstructed image.
  
- **Quantitative Comparison of Superresolution** : The above only helps us with a qualitative comparison. Let us now do a quantitative comparison. First read this article: https://github.com/sgrvinod/a-PyTorch-Tutorial-to-Super-Resolution
    - Start with a 400x400 image (ground truth high resolution).
    - Resize it to a 200x200 image (input image)
    - Use `RFF` + `Linear regression` to increase the resolution to 400x400 (predicted high resolution image)
    - Compute the following metrics:
        - `RMSE` on predicted v/s ground truth high resolution image
        - `Peak SNR``
- **Completing Image with Random Missing Data:** 
  - Applying RFF to complete the image with 10%, 20%, and so on up to 90% of its data missing randomly. 
  - Randomly remove portions of the data, train the model on the remaining data, and predict on the entire image. 
  - Displaying the reconstructed images for each missing data percentage and providing the metrics calculated above.