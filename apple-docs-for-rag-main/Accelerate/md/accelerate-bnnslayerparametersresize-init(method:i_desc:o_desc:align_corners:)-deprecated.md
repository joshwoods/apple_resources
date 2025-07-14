

- Accelerate
- BNNSLayerParametersResize
-  init(method:i_desc:o_desc:align_corners:) Deprecated

Initializer

# init(method:i_desc:o_desc:align_corners:)

Returns a new resize-layer parameters structure from the specified parameters.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
init(
    method: BNNSInterpolationMethod,
    i_desc: BNNSNDArrayDescriptor,
    o_desc: BNNSNDArrayDescriptor,
    align_corners: Bool
)
```

Deprecated

Use BNNSGraph\* APIs

## Parameters 

`method`  

The interpolation method for resizing.

`i_desc`  

The descriptor of the input.

`o_desc`  

The descriptor of the output.

`align_corners`  

A Boolean value that specifies whether to align the corners of the upscaling grid to the center of scaling dimensions instead of to the edges.

## Discussion

Important

The number of input dimensions must be equal to number of output dimensions. The resize must be in same direction for all dimensions.

## See Also

### Initializers

init()

Returns a new resize-layer parameters structure.

Deprecated

