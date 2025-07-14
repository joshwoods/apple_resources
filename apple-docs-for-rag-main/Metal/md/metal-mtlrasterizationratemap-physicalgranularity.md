

- Metal
- MTLRasterizationRateMap
-  physicalGranularity 

Instance Property

# physicalGranularity

The granularity, in physical pixels, at which the rasterization rate varies.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
var physicalGranularity: MTLSize { get }
```

**Required**

## Discussion

If you’re using a rendering algorithm that uses binning or tiling to partition the rendered image, you may want to use the value of this property to determine your bin sizes.

The depth component of the returned MTLSize structure is always `0`.

## See Also

### Inspecting Geometric and Rendering Properties

var layerCount: Int

The number of layers in the rate map.

**Required**

var screenSize: MTLSize

The logical size, in pixels, of the viewport coordinate system.

**Required**

func physicalSize(layer: Int) -> MTLSize

Returns the dimensions, in pixels, of the area in the render target affected by the rasterization rate map.

**Required**

