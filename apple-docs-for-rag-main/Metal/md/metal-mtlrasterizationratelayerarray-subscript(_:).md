

- Metal
- MTLRasterizationRateLayerArray
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Retrieves the sample value at the specified index.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
subscript(layerIndex: Int) -> MTLRasterizationRateLayerDescriptor? { get set }
```

## Parameters 

`layerIndex`  

The index of the sample you want to retrieve.

## Return Value

An NSNumber instance describing the value of the sample at the specified index, or `0` if the index is out of range.

## See Also

### Accessing Members of the Array

class MTLRasterizationRateLayerDescriptor

The minimum rasterization rates to apply to sections of a layer in the render target.

