

- Accelerate
- BNNS
-  BNNS.ResizeLayer Deprecated

Class

# BNNS.ResizeLayer

A layer object that wraps a resize filter and manages its deinitialization.

iOS 14.0+iPadOS 14.0+Mac CatalystmacOS 11.0+visionOSwatchOS 7.0+tvOS 14.0+

``` source
class ResizeLayer
```

Deprecated

Use the BNNSGraph API instead.

## Topics

### Creating a Resize Layer

convenience init?(interpolationMethod: BNNS.InterpolationMethod, input: BNNSNDArrayDescriptor, output: BNNSNDArrayDescriptor, alignsCorners: Bool, filterParameters: BNNSFilterParameters?)

Returns a new resize layer.

### Specifying an Interpolation Method

enum InterpolationMethod

Constants that specify interpolation methods for resize operations.

## Relationships

### Inherits From

- BNNS.UnaryLayer

## See Also

### Resize layers

struct BNNSInterpolationMethod

Constants that describe interpolation methods.

struct BNNSLayerParametersResize

A structure that contains the parameters of a resize layer.

Deprecated

func BNNSFilterCreateLayerResize(UnsafePointer&lt;BNNSLayerParametersResize>, UnsafePointer&lt;BNNSFilterParameters>?) -> BNNSFilter?

Returns a new resize layer.

Deprecated

