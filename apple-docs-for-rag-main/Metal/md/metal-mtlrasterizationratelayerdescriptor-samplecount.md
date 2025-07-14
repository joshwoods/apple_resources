

- Metal
- MTLRasterizationRateLayerDescriptor
-  sampleCount 

Instance Property

# sampleCount

The number of rows and columns in the layer map.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
var sampleCount: MTLSize { get set }
```

## Discussion

The sampleCount property splits the logical viewport coordinate space into a 2D grid of equal-sized cells. Its depth value is always `0`.

The default value is the same as maxSampleCount.

## See Also

### Inspecting the Layer Rate Function Parameters

var maxSampleCount: MTLSize

The maximum number of rows and columns in the layer map.

var horizontal: MTLRasterizationRateSampleArray

The horizontal rasterization rates for the layer map’s rows.

var vertical: MTLRasterizationRateSampleArray

The vertical rasterization rates for the layer map’s rows.

class MTLRasterizationRateSampleArray

An array object that contains rasterization rates.

