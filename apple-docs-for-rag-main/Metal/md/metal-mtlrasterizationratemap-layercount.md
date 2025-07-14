

- Metal
- MTLRasterizationRateMap
-  layerCount 

Instance Property

# layerCount

The number of layers in the rate map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
var layerCount: Int { get }
```

**Required**

## See Also

### Inspecting Geometric and Rendering Properties

var screenSize: MTLSize

The logical size, in pixels, of the viewport coordinate system.

**Required**

func physicalSize(layer: Int) -> MTLSize

Returns the dimensions, in pixels, of the area in the render target affected by the rasterization rate map.

**Required**

var physicalGranularity: MTLSize

The granularity, in physical pixels, at which the rasterization rate varies.

**Required**

