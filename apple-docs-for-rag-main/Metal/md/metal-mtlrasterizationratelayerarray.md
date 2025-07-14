

- Metal
-  MTLRasterizationRateLayerArray 

Class

# MTLRasterizationRateLayerArray

Descriptions for the rasterization rates to apply to the set of layers in a rate map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
class MTLRasterizationRateLayerArray
```

## Topics

### Accessing Members of the Array

subscript(Int) -> MTLRasterizationRateLayerDescriptor?

Retrieves the sample value at the specified index.

class MTLRasterizationRateLayerDescriptor

The minimum rasterization rates to apply to sections of a layer in the render target.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuring the Rate Map Layers

var layerCount: Int

The number of layers in the rate map.

func layer(at: Int) -> MTLRasterizationRateLayerDescriptor?

Returns the layer description for a layer in the rate map.

func setLayer(MTLRasterizationRateLayerDescriptor?, at: Int)

Sets a configuration for a layer rate map.

var layers: MTLRasterizationRateLayerArray

The rasterization rates for one or more layers in the rate map.

