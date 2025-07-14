

- Metal
- MTLRasterizationRateMapDescriptor
-  layers 

Instance Property

# layers

The rasterization rates for one or more layers in the rate map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
var layers: MTLRasterizationRateLayerArray { get }
```

## See Also

### Configuring the Rate Map Layers

var layerCount: Int

The number of layers in the rate map.

func layer(at: Int) -> MTLRasterizationRateLayerDescriptor?

Returns the layer description for a layer in the rate map.

func setLayer(MTLRasterizationRateLayerDescriptor?, at: Int)

Sets a configuration for a layer rate map.

class MTLRasterizationRateLayerArray

Descriptions for the rasterization rates to apply to the set of layers in a rate map.

