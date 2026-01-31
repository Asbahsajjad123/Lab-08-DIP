# Lab-08-DIP
1.	Add noise: Gaussian, salt & pepper, motion blur.
2.	Apply median, Wiener, and inverse filtering.
3.	Restore motion-blurred image.
4.	Compute PSNR.
5.	Identify best restoration method for each noise type.
# Code Explanation
This code demonstrates image degradation and restoration techniques using Python in Google Colab. First, a grayscale image is uploaded at runtime, read using OpenCV, and normalized to values between 0 and 1. A helper function is defined to visually compare the original image, the degraded (noisy or blurred) image, and the restored result. Gaussian noise is added to the image and then removed using a Wiener filter, which reduces noise by considering both the noise level and the blurring function. Next, salt-and-pepper noise is introduced, and a median filter is applied to restore the image by effectively removing impulse noise. After that, motion blur is simulated using a linear kernel, and the blurred image is restored using Wiener (inverse) filtering. To evaluate the quality of restoration, Peak Signal-to-Noise Ratio (PSNR) is calculated for each restored image, providing a numerical measure of how close the restored image is to the original. Finally, all restoration results are displayed and their PSNR values are printed for comparison.
