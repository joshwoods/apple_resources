

- Metal
- MTLDevice
-  supportsRasterizationRateMap(layerCount:) 

Instance Method

# supportsRasterizationRateMap(layerCount:)

Returns a Boolean value that indicates whether the GPU can create a rasterization rate map with a specific number of layers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
func supportsRasterizationRateMap(layerCount: Int) -> Bool
```

**Required**

## Parameters 

`layerCount`  

The number of layers for a rasterization rate map.

## See Also

### Creating Rasterization Rate Maps

func makeRasterizationRateMap(descriptor: MTLRasterizationRateMapDescriptor) -> (any MTLRasterizationRateMap)?

Creates a rasterization rate map instance.

**Required**

