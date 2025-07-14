

- Metal
- MTLRasterizationRateLayerDescriptor
-  maxSampleCount 

Instance Property

# maxSampleCount

The maximum number of rows and columns in the layer map.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var maxSampleCount: MTLSize { get }
```

## Discussion

Its depth value is always `0`.

## See Also

### Inspecting the Layer Rate Function Parameters

var sampleCount: MTLSize

The number of rows and columns in the layer map.

var horizontal: MTLRasterizationRateSampleArray

The horizontal rasterization rates for the layer map’s rows.

var vertical: MTLRasterizationRateSampleArray

The vertical rasterization rates for the layer map’s rows.

class MTLRasterizationRateSampleArray

An array object that contains rasterization rates.

