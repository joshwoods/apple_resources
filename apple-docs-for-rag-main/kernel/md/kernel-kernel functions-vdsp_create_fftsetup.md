

- Kernel
- Kernel Functions
-  vDSP_create_fftsetup 

Function

# vDSP_create_fftsetup

Returns a setup structure that contains precalculated data for single-precision FFT functions.

macOS 10.0+

``` source
FFTSetup vDSP_create_fftsetup(vDSP_Length __Log2n, FFTRadix __Radix);
```

## Parameters 

`__Log2n`  

The base-two logarithm of the maximum number of elements the setup structure transforms. Subsequent calls to FFT functions using the resulting setup may transform this length or less.

`__Radix`  

Specifies radix options. This function only supports radix-2; other radices are deprecated. Use the Discrete Fourier transforms for radix-3, and radix-5.

## Return Value

Returns an FFTSetup structure for use with FFT functions. Returns `0` on error.

## Discussion

Use this function to create a weights array of complex exponential values that the vDSP FFT functions use for forward transforms. Precalculating these values during, for example, your app’s initialization, boosts FFT performance. You can use the same setup structure to perform transforms on vectors that contain up to `2`Log2n elements.

For 2D transforms, specify `Log2n` as the greater of the number of rows and the number of columns.

Call vDSP_destroy_fftsetup to deallocate the setup structure.

