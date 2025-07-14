

- Metal
- MTLRasterizationRateLayerDescriptor
-  init(horizontal:vertical:) 

Initializer

# init(horizontal:vertical:)

Initializes a layer rate map with a set of horizontal and vertical rasterization rates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS

``` source
convenience init(
    horizontal: [Float],
    vertical: [Float]
)
```

## Parameters 

`horizontal`  

An array of the horizontal rates to apply across the grid.

`vertical`  

An array of the vertical rates to apply across the grid.

## Return Value

A layer descriptor whose width is the number of horizontal rates and whose height is the number of vertical rates. The layer descriptor copies the values from the input parameters.

## See Also

### Creating a Layer Rasterization Rate Descriptor

init(sampleCount: MTLSize)

Initializes the layer map with an empty grid.

