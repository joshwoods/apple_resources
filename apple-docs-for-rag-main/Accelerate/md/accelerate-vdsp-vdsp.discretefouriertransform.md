

- Accelerate
- vDSP
-  vDSP.DiscreteFourierTransform 

Class

# vDSP.DiscreteFourierTransform

An object that provides forward and inverse discrete Fourier transforms on single- or double-precision collections of interleaved or split-complex data.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
class DiscreteFourierTransform where T : vDSP_DiscreteFourierTransformable
```

## Overview

Use a vDSP.DiscreteFourierTransform to perform discrete Fourier transforms (DFTs) on split-complex or interleaved data. To learn more about working with split-complex and interleaved data, see Performing Fourier transforms on interleaved-complex data.

To create a vDSP.DiscreteFourierTransform instance to work with interleaved data, pass either DSPComplex or DSPDoubleComplex to init(previous:count:direction:transformType:ofType:). The following code shows how to perform a forward complex-to-complex DFT on the interleaved single-precision values in the `interleavedInput` array:

```
// The `interleavedInput` array contains `complexValuesCount` `DSPComplex` elements.
let interleavedInput: [DSPComplex] = [ ... ]

let interleavedDFT = try? vDSP.DiscreteFourierTransform(previous: nil,
                                                        count: complexValuesCount,
                                                        direction: .forward,
                                                        transformType: .complexComplex,
                                                        ofType: DSPComplex.self)

// On return, the `interleavedOutput` array contains an array of `DSPComplex`
// structures.
let interleavedOutput = interleavedDFT?.transform(input: interleavedInput)
```

To create a vDSP.DiscreteFourierTransform instance to work with split-complex data, pass either Float or Double to init(previous:count:direction:transformType:ofType:). Split-complex data stores the real and imaginary parts of each complex value in separate arrays. The following code shows how to perform forward complex-to-complex DFT on the split-complex single-precision values in the `splitComplexRealInput` and `splitComplexImaginaryInput` arrays:

```
var splitComplexRealInput: [Float] = [ ... ]
var splitComplexImaginaryInput: [Float] = [ ... ]

let splitComplexDFT = try? vDSP.DiscreteFourierTransform(previous: nil,
                                                         count: complexValuesCount,
                                                         direction: .forward,
                                                         transformType: .complexComplex,
                                                         ofType: Float.self)

// The `splitComplexOutput` tuple contains two arrays that represent the
// real and imaginary parts of the output.
let splitComplexOutput = splitComplexDFT?.transform(real: splitComplexRealInput,
                                                    imaginary: splitComplexImaginaryInput)
```

If the underlying data in both the `interleavedInput` array and the split-complex input arrays is the same, for each `i` in `0 ..

```
interleavedOutput[i].real ≈ splitComplexOutput.real[i]
interleavedOutput[i].imag ≈ splitComplexOutput.imaginary[i]
```

\`\`

## Topics

### Creating a Discrete Fourier Transform Instance

init(previous: vDSP.DiscreteFourierTransform&lt;Float>?, count: Int, direction: vDSP.FourierTransformDirection, transformType: vDSP.DFTTransformType, ofType: T.Type) throws

Returns a new discrete Fourier transform instance.

### Performing Split-Complex Discrete Fourier Transforms

func transform&lt;U>(real: U, imaginary: U) -> (real: [Float], imaginary: [Float])

Returns the result of a single-precision discrete Fourier transform.

func transform&lt;U>(real: U, imaginary: U) -> (real: [Double], imaginary: [Double])

Returns the result of a double-precision discrete Fourier transform.

func transform&lt;U, V>(inputReal: U, inputImaginary: U, outputReal: inout V, outputImaginary: inout V)

Computes a single-precision discrete Fourier transform.

func transform&lt;U, V>(inputReal: U, inputImaginary: U, outputReal: inout V, outputImaginary: inout V)

Computes a double-precision discrete Fourier transform.

### Performing Interleaved Discrete Fourier Transforms

func transform&lt;U>(input: U) -> [DSPComplex]

Returns the result of a single-precision discrete Fourier transform.

func transform&lt;U>(input: U) -> [DSPDoubleComplex]

Returns the result of a double-precision discrete Fourier transform.

func transform&lt;U, V>(input: U, output: inout V)

Computes a single-precision discrete Fourier transform.

func transform&lt;U, V>(input: U, output: inout V)

Computes a double-precision discrete Fourier transform.

## See Also

### Objects that simplify discrete Fourier transforms

enum DFTTransformType

Discrete Fourier transform types.

class DFT

A single- and double-precision discrete Fourier transform.

Deprecated

