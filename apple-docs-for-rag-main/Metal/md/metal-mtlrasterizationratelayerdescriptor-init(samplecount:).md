

- Metal
- MTLRasterizationRateLayerDescriptor
-  init(sampleCount:) 

Initializer

# init(sampleCount:)

Initializes the layer map with an empty grid.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
init(sampleCount: MTLSize)
```

## Parameters 

`sampleCount`  

The size of the grid. Specify the width and height to determine the number of columns and rows in the layer map. The initializer ignores the depth component.

## Return Value

A layer descriptor with a grid of the specified size. All of the rasterization rates are set to `0.0`.

## See Also

### Creating a Layer Rasterization Rate Descriptor

convenience init(horizontal: [Float], vertical: [Float])

Initializes a layer rate map with a set of horizontal and vertical rasterization rates.

