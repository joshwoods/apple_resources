

- Accelerate
-  BNNSLayerParametersResize Deprecated

Structure

# BNNSLayerParametersResize

A structure that contains the parameters of a resize layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersResize
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(method: BNNSInterpolationMethod, i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, align_corners: Bool)

Returns a new resize-layer parameters structure from the specified parameters.

init()

Returns a new resize-layer parameters structure.

### Instance Properties

var method: BNNSInterpolationMethod

The interpolation method for resizing.

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var align_corners: Bool

A Boolean value that specifies whether to align the corners of the upscaling grid to the center of scaling dimensions instead of to the edges.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Resize layers

class ResizeLayer

A layer object that wraps a resize filter and manages its deinitialization.

Deprecated

struct BNNSInterpolationMethod

Constants that describe interpolation methods.

func BNNSFilterCreateLayerResize(UnsafePointer&lt;BNNSLayerParametersResize>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new resize layer.

Deprecated

