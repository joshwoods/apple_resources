

- Accelerate
- BNNS
-  BNNS.PaddingLayer Deprecated

Class

# BNNS.PaddingLayer

A layer object that wraps a padding filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+macOS 11.0+tvOS 14.0+visionOSwatchOS 7.0+Mac Catalyst

``` source
class PaddingLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Padding Layer

convenience init?(input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, mode: BNNS.PaddingMode, size: [(x: Int, y: Int)], filterParameters: BNNSFilterParameters?)

Returns a new padding layer.

### Specifying the Padding Mode

enum PaddingMode

Constants that define padding modes.

## Relationships

### Inherits From

- BNNS.UnaryLayer

## See Also

### Padding layers

struct BNNSPaddingMode

Constants that define padding modes.

struct BNNSLayerParametersPadding

A structure that contains the parameters of a padding layer.

Deprecated

func BNNSFilterCreateLayerPadding(UnsafePointer&lt;BNNSLayerParametersPadding>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new loss layer.

Deprecated

