

- Accelerate
- vDSP
- vDSP.DiscreteFourierTransform
-  init(previous:count:direction:transformType:ofType:) 

Initializer

# init(previous:count:direction:transformType:ofType:)

Returns a new discrete Fourier transform instance.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
init(
    previous: vDSP.DiscreteFourierTransform? = nil,
    count: Int,
    direction: vDSP.FourierTransformDirection,
    transformType: vDSP.DFTTransformType,
    ofType: T.Type
) throws
```

## Parameters 

`previous`  

An existing vDSP.DiscreteFourierTransform structure that shares memory with the discrete Fourier transform instance that this function returns. Pass `nil` to create an object with newly initialized and allocated memory.

`count`  

The number of complex elements. For split-complex real-to-complex, the value of count must be `2ⁿ` or `f * 2ⁿ`, where `f` is `3`, `5`, or `15` and `n >= 4`. For split-complex complex-to-complex, the value of count must be `2ⁿ` or `f * 2ⁿ`, where `f` is `3`, `5`, or `15` and `n >= 3`. And for interleaved, the value of count must be `f * 2ⁿ`, where `f` is `2`, `3`, `5`, `3 * 3`, `3 x 5`, or `5 * 5`, and `n>=2`.

`direction`  

A flag that specifies the transform direction.

`transformType`  

A flag that specifies whether the forward transform is real-to-complex or complex-to-complex.

`ofType`  

The data type for the discrete Fourier transform operation. For split-complex operations, this must be either Float or Double. For interleaved operations, this must be either DSPComplex or DSPDoubleComplex.

