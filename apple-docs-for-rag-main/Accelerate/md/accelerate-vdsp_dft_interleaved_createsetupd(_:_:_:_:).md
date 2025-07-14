

- Accelerate
-  vDSP_DFT_Interleaved_CreateSetupD(\_:\_:\_:\_:) 

Function

# vDSP_DFT_Interleaved_CreateSetupD(\_:\_:\_:\_:)

Returns a setup structure that contains precalculated data for forward and inverse, double-precision interleaved discrete Fourier transform (DFT) functions.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func vDSP_DFT_Interleaved_CreateSetupD(
    _ Previous: vDSP_DFT_Interleaved_SetupD?,
    _ Length: vDSP_Length,
    _ Direction: vDSP_DFT_Direction,
    _ RealtoComplex: vDSP_DFT_RealtoComplex
) -> vDSP_DFT_Interleaved_SetupD?
```

## Parameters 

`Previous`  

An existing vDSP_DFT_Interleaved_SetupD structure that shares memory and direction with the setup structure that this function returns. Pass `nil` to create an object with newly initialized and allocated memory. To ensure correct operation, if you specify a previous setup structure it must share the same direction as the `Direction` parameter.

`Length`  

For complex-to-complex transforms, the number of complex elements.

For real-to-complex transforms, the number of real elements divided by 2.

`Direction`  

A flag that specifies the transform direction. Pass vDSP_DFT_Direction.FORWARD to transform from the time domain to the frequency domain. Pass vDSP_DFT_Direction.INVERSE to transform from the frequency domain to the time domain.

`RealtoComplex`  

A flag that specifies the transform type. To transform from complex to complex, pass vDSP_DFT_RealtoComplex.interleaved_ComplextoComplex. To transform from real to complex, pass vDSP_DFT_RealtoComplex.interleaved_RealtoComplex.

## Return Value

Returns a vDSP_DFT_Interleaved_SetupD object, or `nil` if the function fails, either from insufficient memory or because `Length` doesn’t satisfy the above requirements.

## Discussion

Important

To prevent potential memory leaks, if the `Previous` parameter is not `nil`, the return value and the `Previous` value must be different variables.

## Discussion

The interleaved DFT operations that the Accelerate framework provides work over collections with specific counts. The maximum number of complex elements that these operations support is 4,096, and other supported counts are the result of the formula `f * 2ⁿ` for certain values of `f` and `n`. In the case of real-to-complex, `n` is the number of real elements divided by two, and for complex-to-complex `n` is the number of complex elements.

The following tables show the complete list of supported lengths for different values of `f` and `n`.

### Supported lengths for f = 1

| n   | `2ⁿ`  | `length` (`f * 2ⁿ`) |
|-----|-------|---------------------|
| 3   | 8     | **8**               |
| 4   | 16    | **16**              |
| 5   | 32    | **32**              |
| 6   | 64    | **64**              |
| 7   | 128   | **128**             |
| 8   | 256   | **256**             |
| 9   | 512   | **512**             |
| 10  | 1,024 | **1,024**           |
| 11  | 2,048 | **2,048**           |
| 12  | 4,096 | **4,096**           |

### Supported lengths for f = 3

| n   | `2ⁿ` | `length` (`f * 2ⁿ`) |
|-----|------|---------------------|
| 2   | 4    | **12**              |
| 3   | 8    | **24**              |
| 4   | 16   | **48**              |
| 5   | 32   | **96**              |
| 6   | 64   | **192**             |
| 7   | 128  | **384**             |
| 8   | 256  | **768**             |

### Supported lengths for f = 5

| n   | `2ⁿ` | `length` (`f * 2ⁿ`) |
|-----|------|---------------------|
| 2   | 4    | **20**              |
| 3   | 8    | **40**              |
| 4   | 16   | **80**              |
| 5   | 32   | **160**             |
| 6   | 64   | **320**             |
| 7   | 128  | **640**             |

### Supported lengths for f = 9

| n   | `2ⁿ` | `length` (`f * 2ⁿ`) |
|-----|------|---------------------|
| 2   | 4    | **36**              |
| 3   | 8    | **72**              |
| 4   | 16   | **144**             |
| 5   | 32   | **288**             |
| 6   | 64   | **576**             |
| 7   | 128  | **1,152**           |

### Supported lengths for f = 15

| n   | `2ⁿ` | `length` (`f * 2ⁿ`) |
|-----|------|---------------------|
| 2   | 4    | **60**              |
| 3   | 8    | **120**             |
| 4   | 16   | **240**             |
| 5   | 32   | **480**             |
| 6   | 64   | **960**             |
| 7   | 128  | **1,920**           |

## See Also

### Related Documentation

Understanding data packing for Fourier transforms

Format source data for the vDSP Fourier functions, and interpret the results.

Reducing spectral leakage with windowing

Multiply signal data by window sequence values when performing transforms with noninteger period signals.

### Interleaved discrete Fourier transform functions

Performing Fourier transforms on interleaved-complex data

Optimize discrete Fourier transform (DFT) performance with the vDSP interleaved DFT routines.

func vDSP_DFT_Interleaved_CreateSetup(vDSP_DFT_Interleaved_Setup?, vDSP_Length, vDSP_DFT_Direction, vDSP_DFT_RealtoComplex) -> vDSP_DFT_Interleaved_Setup?

Returns a setup structure that contains precalculated data for forward and inverse, single-precision interleaved discrete Fourier transform (DFT) functions.

func vDSP_DFT_Interleaved_Execute(vDSP_DFT_Interleaved_Setup, UnsafePointer&lt;DSPComplex>, UnsafeMutablePointer&lt;DSPComplex>)

Calculates the single-precision discrete Fourier transform (DFT) for a vector of interleaved complex values.

func vDSP_DFT_Interleaved_ExecuteD(vDSP_DFT_Interleaved_SetupD, UnsafePointer&lt;DSPDoubleComplex>, UnsafeMutablePointer&lt;DSPDoubleComplex>)

Calculates the double-precision discrete Fourier transform (DFT) for a vector of interleaved complex values.

func vDSP_DFT_Interleaved_DestroySetup(vDSP_DFT_Interleaved_Setup?)

Releases a single-precision discrete Fourier transform (DFT) setup structure.

func vDSP_DFT_Interleaved_DestroySetupD(vDSP_DFT_Interleaved_SetupD?)

Releases a double-precision discrete Fourier transform (DFT) setup structure.

