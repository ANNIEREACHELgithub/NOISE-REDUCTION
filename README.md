Importing and Reading Audio Signal: The project begins by importing an audio signal and reading it using Python libraries such as SciPy or librosa.
Denoising Data with FFT Algorithm: The core of the project involves denoising the audio data using the Fast Fourier Transform (FFT) algorithm. FFT is utilized to transform the audio signal from the time domain to the frequency domain, where noise can be effectively identified and removed.
Band Limiting Noise: Band-limiting noise involves defining specific frequency bands where noise is expected to occur, allowing for more targeted denoising efforts.
Adding Noise: In order to test the denoising capabilities of the algorithm, noise is intentionally added to the original audio signal.
Creating a Mask: A mask is generated by comparing the FFT of the signal with a calculated threshold, identifying areas with significant noise presence.
Applying Short Time Fourier Transform (STFT): STFT is applied to the audio signal to analyze its frequency content over time, facilitating a more detailed examination of noise characteristics.
Creating a Smoothing Filter for the Mask: Smoothing filters are employed to refine the mask, enhancing its precision in identifying noise components across both frequency and time dimensions.
Convolution of the Mask with a Smoothing Filter: Convolution is used to combine the mask with the smoothing filter, further refining its effectiveness in noise identification.
Calculating the Threshold: The threshold is determined based on statistical analysis of the noise, as well as the desired sensitivity level of the denoising algorithm.
Plotting the Spectrogram: Spectrograms are plotted to visualize the frequency content of the audio signal and the effectiveness of the denoising process.
Masking Signals Above the Threshold: Signals above the calculated threshold are masked, indicating areas where noise removal is necessary.
Denoising Noise Above the Threshold Limit: Finally, noise above the threshold limit is effectively removed from the audio signal using the derived mask and FFT inversion techniques.
