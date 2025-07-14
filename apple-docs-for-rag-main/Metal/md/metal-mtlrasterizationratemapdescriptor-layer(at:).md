

- Metal
- MTLRasterizationRateMapDescriptor
-  layer(at:) 

Instance Method

# layer(at:)

Returns the layer description for a layer in the rate map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
func layer(at layerIndex: Int) -> MTLRasterizationRateLayerDescriptor?
```

## Parameters 

`layerIndex`  

The entry to return.

## Return Value

The MTLRasterizationRateLayerDescriptor instance for the given index, or `nil` if you haven’t set an instance for this index.

## Discussion

Calling this method is equivalent to using array subscript syntax.

## See Also

### Configuring the Rate Map Layers

var layerCount: Int

The number of layers in the rate map.

func setLayer(MTLRasterizationRateLayerDescriptor?, at: Int)

Sets a configuration for a layer rate map.

var layers: MTLRasterizationRateLayerArray

The rasterization rates for one or more layers in the rate map.

class MTLRasterizationRateLayerArray

Descriptions for the rasterization rates to apply to the set of layers in a rate map.

