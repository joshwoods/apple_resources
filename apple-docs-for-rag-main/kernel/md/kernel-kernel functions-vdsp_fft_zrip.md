

- Kernel
- Kernel Functions
-  vDSP_fft_zrip 

Function

# vDSP_fft_zrip

Computes a forward or inverse in-place, single-precision real FFT.

macOS 10.0+

``` source
void vDSP_fft_zrip(FFTSetup __Setup, const DSPSplitComplex *__C, vDSP_Stride __IC, vDSP_Length __Log2N, FFTDirection __Direction);
```

## Parameters 

`__Setup`  

The FFT setup structure for this transform. The setup’s structure `Log2N` must be greater than or equal to this function’s `Log2N`.

`__C`  

A pointer to the input-output data.

`__IC`  

The stride between the elements in `C`, set to 1 for best performance.

`__Log2N`  

The base 2 exponent of the number of elements to process. For example, to process 1024 elements, specify 10 for parameter `Log2N`.

`__Direction`  

A flag that specifies the transform direction. Pass kFFTDirection_Forward to transform from the time domain to the frequency domain. Pass kFFTDirection_Inverse to transform from the frequency domain to the time domain.

## Discussion

Forward transforms read real input and write packed complex output. Inverse transforms read packed complex input and write real output. As a result of packing the frequency-domain data, time-domain data and its equivalent frequency-domain data have the same storage requirements. You can find more details on the packing format in Data Packing for Real FFTs in vDSP Programming Guide.

where F is `Direction`, C is `C`, and N is two raised to the power of `Log2N`.

See also functions vDSP_create_fftsetup and vDSP_destroy_fftsetup.

