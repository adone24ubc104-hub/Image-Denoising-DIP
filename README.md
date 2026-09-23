# Image Denoising Using Spatial Filtering Techniques

## Digital Image Processing Mini Project

### Project Overview

This project investigates image denoising using spatial filtering techniques. Two types of artificial noise, Gaussian noise and salt-and-pepper noise, are introduced into original RGB images. Three spatial filtering techniques are then applied to reduce the noise:

* Mean Filter
* Median Filter
* Gaussian Filter

The performance of the filtering techniques is evaluated using Mean Squared Error (MSE), Peak Signal-to-Noise Ratio (PSNR), and Structural Similarity Index (SSIM).

The experiment is first demonstrated using an individual image and is then extended to multiple uploaded images. Average performance values are calculated to compare the filtering techniques under different noise conditions.

---

## Objectives

The main objectives of this project are:

1. To study the effect of artificial noise on digital images.
2. To simulate Gaussian and salt-and-pepper noise.
3. To implement different spatial filtering techniques.
4. To compare mean, median, and Gaussian filtering.
5. To evaluate denoising performance using MSE, PSNR, and SSIM.
6. To perform the experiment on multiple images and calculate average results.
7. To visualize and compare the performance of the filtering techniques.

---

## Methodology

The project follows the following processing pipeline:

```text
Original Image
      ↓
Image Resizing
      ↓
Noise Addition
 ┌────┴─────────────┐
 ↓                  ↓
Gaussian Noise   Salt-and-Pepper
 ↓                  ↓
Spatial Filtering  Spatial Filtering
 ↓                  ↓
Mean / Median / Gaussian Filters
 └────────┬─────────┘
          ↓
Image Quality Evaluation
          ↓
MSE / PSNR / SSIM
          ↓
Comparison of Results
          ↓
Average Results Across Images
```

### Image Preprocessing

The input RGB images are resized to 512 × 512 pixels to maintain a consistent image size during processing.

### Noise Generation

Two artificial noise models are used:

* Gaussian noise with mean = 0 and standard deviation = 25.
* Salt-and-pepper noise with an amount of 0.05.

### Spatial Filtering

Three filters are applied:

* Mean filtering using a 5 × 5 kernel.
* Median filtering using a kernel size of 5.
* Gaussian filtering using a 5 × 5 kernel.

### Performance Evaluation

The filtered images are compared with the corresponding original images using:

* MSE
* PSNR
* SSIM

The experiment is repeated for all uploaded images, and average values are calculated for each noise-filter combination.

---

## Evaluation Metrics

### Mean Squared Error (MSE)

MSE measures the average squared difference between the original image and the restored image. A lower MSE represents a smaller reconstruction error.

### Peak Signal-to-Noise Ratio (PSNR)

PSNR is used to measure the quality of the restored image relative to the original image. Higher PSNR values generally indicate better image restoration.

### Structural Similarity Index (SSIM)

SSIM measures the structural similarity between the original and restored images. Values closer to 1 indicate greater structural similarity.

---

## Technologies Used

* Python
* Google Colab
* OpenCV
* NumPy
* Pandas
* Matplotlib
* scikit-image

---

## Repository Contents

| File                        | Description                                 |
| --------------------------- | ------------------------------------------- |
| `Dip_mini_project.ipynb`    | Complete Python/Google Colab implementation |
| `final_average_results.csv` | Average MSE, PSNR and SSIM results          |
| `all_image_results.csv`     | Detailed results for individual images      |
| `average_mse.png`           | Average MSE comparison graph                |
| `average_psnr.png`          | Average PSNR comparison graph               |
| `average_ssim.png`          | Average SSIM comparison graph               |

---

## How to Run

1. Open `Dip_mini_project.ipynb` using Google Colab.
2. Run the notebook from the beginning.
3. Upload the required input images when prompted.
4. The notebook adds Gaussian and salt-and-pepper noise.
5. Mean, median, and Gaussian filters are applied.
6. MSE, PSNR, and SSIM are calculated.
7. The experiment is repeated for all uploaded images.
8. Average results are generated.
9. Comparison graphs are produced.

---

## Results

The project produces quantitative results for each combination of noise type and filtering technique.

The final average results are available in:

`final_average_results.csv`

Detailed image-wise results are available in:

`all_image_results.csv`

The repository also contains graphical comparisons of:

* Average MSE
* Average PSNR
* Average SSIM

These results are used to analyze the effectiveness of the different spatial filtering techniques.

---

## Conclusion

This project demonstrates the application of spatial filtering techniques for image denoising. Gaussian and salt-and-pepper noise are introduced into original images, followed by restoration using mean, median, and Gaussian filters. MSE, PSNR, and SSIM are used to quantitatively evaluate the resulting images. The multi-image experiment provides an overall comparison of the filtering techniques under the two noise conditions.

---

## Project Type

**Digital Image Processing Mini Project**

**Topic:** Image Denoising Using Spatial Filtering Techniques
