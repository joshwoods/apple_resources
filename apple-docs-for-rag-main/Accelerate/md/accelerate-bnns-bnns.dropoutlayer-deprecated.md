

- Accelerate
- BNNS
-  BNNS.DropoutLayer Deprecated

Class

# BNNS.DropoutLayer

A layer object that wraps a dropout filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
class DropoutLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Dropout Layer

convenience init?(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, rate: Float, seed: UInt32, control: UInt8, filterParameters: BNNSFilterParameters?)

Returns a new dropout layer.

## Relationships

### Inherits From

- BNNS.UnaryLayer

## See Also

### Dropout layers

struct BNNSLayerParametersDropout

A structure that contains the parameters of a dropout layer.

Deprecated

func BNNSFilterCreateLayerDropout(UnsafePointer&lt;BNNSLayerParametersDropout>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new dropout layer.

Deprecated

