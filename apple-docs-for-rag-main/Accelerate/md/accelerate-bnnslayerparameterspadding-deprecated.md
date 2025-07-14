

- Accelerate
-  BNNSLayerParametersPadding Deprecated

Structure

# BNNSLayerParametersPadding

A structure that contains the parameters of a padding layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersPadding
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, padding_size: ((Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int)), padding_mode: BNNSPaddingMode, padding_value: UInt32)

Returns a new padding-layer parameters structure from the specified parameters.

init()

Returns a new padding-layer parameters structure.

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var padding_size: ((Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int), (Int, Int))

The number of padding elements to add before and after the original data.

var padding_mode: BNNSPaddingMode

The mode the operation uses to pad.

var padding_value: UInt32

The value the operation uses to fill the padding area when the mode is constant.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Padding layers

class PaddingLayer

A layer object that wraps a padding filter and manages its deinitialization.

Deprecated

struct BNNSPaddingMode

Constants that define padding modes.

func BNNSFilterCreateLayerPadding(UnsafePointer&lt;BNNSLayerParametersPadding>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new loss layer.

Deprecated

