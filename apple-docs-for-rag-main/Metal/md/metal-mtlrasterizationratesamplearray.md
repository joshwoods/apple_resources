

- Metal
-  MTLRasterizationRateSampleArray 

Class

# MTLRasterizationRateSampleArray

An array object that contains rasterization rates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.4+macOS 10.15.4+tvOS 16.0+visionOS 1.0+

``` source
class MTLRasterizationRateSampleArray
```

## Overview

The horizontal and vertical properties of a MTLRasterizationRateLayerDescriptor point to MTLRasterizationRateSampleArray objects that contains rasterization rates for the layer map. You can use array subscript syntax to access the samples. MTLRasterizationRateSampleArray objects perform bounds checking on any accesses you make to their sample data.

## Topics

### Accessing the Array

subscript(Int) -> Float

Retrieves the sample value at the specified index.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Inspecting the Layer Rate Function Parameters

var sampleCount: MTLSize

The number of rows and columns in the layer map.

var maxSampleCount: MTLSize

The maximum number of rows and columns in the layer map.

var horizontal: MTLRasterizationRateSampleArray

The horizontal rasterization rates for the layer map’s rows.

var vertical: MTLRasterizationRateSampleArray

The vertical rasterization rates for the layer map’s rows.

