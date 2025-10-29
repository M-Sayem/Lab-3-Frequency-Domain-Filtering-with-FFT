# Lab 3: Frequency-Domain Filtering with FFT

This lab explores image filtering in the frequency domain using the 2D Fourier Transform (`fft2`) and its relationship to spatial convolution.

## Sections

1. **Magnitude Spectrum:** Visualizes the centered frequency components of an image using a log-scaled spectrum.
2. **Low-Pass Filters:** Compares an ideal (hard cutoff) and a Gaussian (smooth) low-pass filter. The ideal LP shows ringing (Gibbs phenomenon), while the Gaussian avoids it.
3. **Frequency-Domain Filtering:** Demonstrates filtering via multiplication in the frequency domain and reconstruction using `ifft2`.
4. **High-Pass Filter:** Obtained as the complement of the Gaussian LP to highlight edges and fine details.
5. **Spatial vs Frequency Comparison:** Shows that Gaussian filters produce nearly identical results whether applied spatially (`imfilter`) or in the frequency domain (`fft2`).
6. **Reflections:**
   - Sharp frequency cutoffs cause ringing due to truncation in frequency.
   - `fftshift` centers the low-frequency components for easier visualization.
   - FFT-based filtering is more efficient for large kernels compared to spatial convolution.

