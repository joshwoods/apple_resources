

- Accelerate
- BNNS
- BNNS.ResizeLayer
-  init(interpolationMethod:input:output:alignsCorners:filterParameters:) Deprecated

Initializer

# init(interpolationMethod:input:output:alignsCorners:filterParameters:)

Returns a new resize layer.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+

``` source
convenience init?(
    interpolationMethod: BNNS.InterpolationMethod,
    input: BNNSNDArrayDescriptor,
    output: BNNSNDArrayDescriptor,
    alignsCorners: Bool,
    filterParameters: BNNSFilterParameters? = nil
)
```

Deprecated

Use the BNNSGraph API instead.

## Parameters 

`interpolationMethod`  

The interpolation method for resizing.

`input`  

The descriptor of the input.

`output`  

The descriptor of the output.

`alignsCorners`  

A Boolean value that specifies whether to align the corners of the upscaling grid to the center of scaling dimensions instead of to the edges.

`filterParameters`  

The filter runtime parameters.

## Discussion

Important

The number of input dimensions must be equal to number of output dimensions. The resize must be in same direction for all dimensions.

