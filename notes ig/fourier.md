# Fourier's Theorem

Say a function $f(t)$ is periodic with period $T$. That is, 

$$f(t) = f(t + T)$$

Then, we can write $f(t)$ as a Fourier series:

$$f(t) = a_0 + \sum_{n=1}^{\infty} a_n \cos(2\pi n t / T) + b_n \sin(2\pi n t / T)$$

where

$$a_0 = \frac{1}{T} \int_{0}^{T} f(t) dt$$

$$a_n = \frac{2}{T} \int_{0}^{T} f(t) \cos(2\pi n t / T) dt$$

$$b_n = \frac{2}{T} \int_{0}^{T} f(t) \sin(2\pi n t / T) dt$$

The Fourier series is a representation of a function as a sum of sines and cosines. The coefficients $a_n$ and $b_n$ are the amplitudes of the sines and cosines, respectively.

The Fourier series is a useful tool for analyzing periodic functions. It allows us to decompose a function into its constituent frequencies and study the behavior of each frequency component separately.

Derivation of the Fourier series: [Proof Document](https://lpsa.swarthmore.edu/Fourier/Series/DerFS.html)

## Example: Square Wave

Consider the square wave function:

$$f(t) = \begin{cases} 1 & \text{if } 0 \leq t < T/2 \\ -1 & \text{if } T/2 \leq t < T \end{cases}$$

The Fourier series of the square wave is given by:

$$f(t) = \frac{4}{\pi} \sum_{n=1}^{\infty} \frac{\sin((2n-1)2\pi t / T)}{2n-1}$$

## Example: Sawtooth Wave

Consider the sawtooth wave function:

$$f(t) = \frac{2t}{T} - 1$$

The Fourier series of the sawtooth wave is given by:

$$f(t) = \sum_{n=1}^{\infty} \frac{2(-1)^{n+1} \sin(2\pi n t / T)}{n}$$

## Example: Triangle Wave

Consider the triangle wave function:

$$f(t) = \begin{cases} 1 - 2t/T & \text{if } 0 \leq t < T/2 \\ -1 + 2t/T & \text{if } T/2 \leq t < T \end{cases}$$

The Fourier series of the triangle wave is given by:

$$f(t) = \sum_{n=0}^{\infty} \frac{8}{\pi^2} \frac{(-1)^n \sin((2n+1)2\pi t / T)}{(2n+1)^2}$$

# Applications of Fourier Series

The Fourier series has many applications in science and engineering. Some of the key applications include:

1. Signal Processing: The Fourier series is used to analyze and process signals in various applications such as audio processing, image processing, and communication systems.

2. Control Systems: The Fourier series is used in the analysis and design of control systems to study the frequency response of the system.

3. Electrical Engineering: The Fourier series is used in the analysis of electrical circuits and systems to study the behavior of signals and waveforms.

4. Quantum Mechanics: The Fourier series is used in quantum mechanics to represent wavefunctions and study the behavior of particles.

5. Data Analysis: The Fourier series is used in data analysis to extract frequency components from signals and study the underlying patterns.

Overall, the Fourier series is a powerful mathematical tool that has a wide range of applications in various fields of science and engineering. It provides a systematic way to analyze and understand the behavior of periodic functions and signals.

## Exponential Form of Fourier Series

The Fourier series can also be expressed in terms of complex exponentials:

$$f(t) = \sum_{n=-\infty}^{\infty} c_n e^{i2\pi n t / T}$$

where

$$c_n = \frac{1}{T} \int_{0}^{T} f(t) e^{-i2\pi n t / T} dt$$

The complex exponential form of the Fourier series is often used in signal processing and communication systems due to its simplicity and compactness.

## Fourier Transform

The Fourier series can be extended to non-periodic functions using the Fourier transform:

$$F(\omega) = \int_{-\infty}^{\infty} f(t) e^{-i\omega t} dt$$

where $F(\omega)$ is the Fourier transform of $f(t)$ and $\omega$ is the frequency variable. The Fourier transform provides a way to analyze the frequency content of non-periodic signals and study their behavior in the frequency domain.

The Fourier transform is a powerful tool in signal processing, communication systems, and quantum mechanics for analyzing signals and wavefunctions in the frequency domain.

What it basically does is fit a function that isn't periodic into a sum of sines and cosines, kind of maybe similar to how Amplitude Modulation works.

## Example: Exponential Fourier Form for Circle

Consider the circle function:

$$f(t) = e^{i\omega t}$$

The exponential Fourier series of the circle function is given by:

$$f(t) = \sum_{n=-\infty}^{\infty} c_n e^{i2\pi n t / T}$$

where

$$c_n = \frac{1}{T} \int_{0}^{T} f(t) e^{-i2\pi n t / T} dt$$



