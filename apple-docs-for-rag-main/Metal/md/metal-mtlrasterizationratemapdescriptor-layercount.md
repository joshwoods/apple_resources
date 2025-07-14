

- Metal
- MTLRasterizationRateMapDescriptor
-  layerCount 

Instance Property

# layerCount

The number of layers in the rate map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
var layerCount: Int { get }
```

## Discussion

The value of this property is dynamically determined based on how many layers you’ve added to the descriptor. To add a new layer, call setLayer(_:at:) or use the subscripting operator to assign a layer.

## See Also

### Configuring the Rate Map Layers

func layer(at: Int) -> MTLRasterizationRateLayerDescriptor?

Returns the layer description for a layer in the rate map.

func setLayer(MTLRasterizationRateLayerDescriptor?, at: Int)

Sets a configuration for a layer rate map.

var layers: MTLRasterizationRateLayerArray

The rasterization rates for one or more layers in the rate map.

class MTLRasterizationRateLayerArray

Descriptions for the rasterization rates to apply to the set of layers in a rate map.

