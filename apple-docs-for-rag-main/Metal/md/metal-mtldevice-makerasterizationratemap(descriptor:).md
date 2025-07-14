

- Metal
- MTLDevice
-  makeRasterizationRateMap(descriptor:) 

Instance Method

# makeRasterizationRateMap(descriptor:)

Creates a rasterization rate map instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
func makeRasterizationRateMap(descriptor: MTLRasterizationRateMapDescriptor) -> (any MTLRasterizationRateMap)?
```

**Required**

## Parameters 

`descriptor`  

An MTLRasterizationRateMapDescriptor instance.

## Return Value

A new MTLRasterizationRateMapDescriptor instance if the method completes successfully; otherwise `nil`.

## See Also

### Creating Rasterization Rate Maps

func supportsRasterizationRateMap(layerCount: Int) -> Bool

Returns a Boolean value that indicates whether the GPU can create a rasterization rate map with a specific number of layers.

**Required**

