

- Metal
- MTLRasterizationRateMapDescriptor
-  setLayer(\_:at:) 

Instance Method

# setLayer(\_:at:)

Sets a configuration for a layer rate map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
func setLayer(
    _ layer: MTLRasterizationRateLayerDescriptor?,
    at layerIndex: Int
)
```

## Parameters 

`layer`  

A description of a layer to add to the rate map descriptor. Use `nil` to remove the layer at that index.

`layerIndex`  

The index to put the new layer description in.

## Discussion

Calling this method is equivalent to using array subscript syntax.

## See Also

### Configuring the Rate Map Layers

var layerCount: Int

The number of layers in the rate map.

func layer(at: Int) -> MTLRasterizationRateLayerDescriptor?

Returns the layer description for a layer in the rate map.

var layers: MTLRasterizationRateLayerArray

The rasterization rates for one or more layers in the rate map.

class MTLRasterizationRateLayerArray

Descriptions for the rasterization rates to apply to the set of layers in a rate map.

