

- Accelerate
-  BNNSLayerParametersDropout Deprecated

Structure

# BNNSLayerParametersDropout

A structure that contains the parameters of a dropout layer.

iOS 14.0–18.0DeprecatediPadOS 14.0–18.0DeprecatedMac Catalyst 14.0–18.0DeprecatedmacOS 11.0–15.0DeprecatedtvOS 14.0–18.0DeprecatedvisionOS 1.0–2.0DeprecatedwatchOS 7.0–11.0Deprecated

``` source
struct BNNSLayerParametersDropout
```

Deprecated

Use BNNSGraph\* APIs

## Topics

### Initializers

init(i_desc: BNNSNDArrayDescriptor, o_desc: BNNSNDArrayDescriptor, rate: Float, seed: UInt32, control: UInt8)

Returns a new dropout layer parameters structure from the specified parameters.

init()

Returns a new dropout layer parameters structure.

### Instance Properties

var i_desc: BNNSNDArrayDescriptor

The descriptor of the input.

var o_desc: BNNSNDArrayDescriptor

The descriptor of the output.

var rate: Float

The probability that the layer drops out an element or a group of elements.

var seed: UInt32

The seed for the random number generator which is ignored if zero.

var control: UInt8

An 8-bit bit mask that indicates the dimension of the grouping of the dropout decision.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Dropout layers

class DropoutLayer

A layer object that wraps a dropout filter and manages its deinitialization.

Deprecated

func BNNSFilterCreateLayerDropout(UnsafePointer&lt;BNNSLayerParametersDropout>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new dropout layer.

Deprecated

