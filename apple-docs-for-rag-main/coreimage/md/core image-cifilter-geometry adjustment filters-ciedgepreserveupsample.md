

- Core Image
- CIFilter
- Geometry Adjustment Filters
-  CIEdgePreserveUpsample 

Protocol

# CIEdgePreserveUpsample

The properties you use to configure an edge preserve upsample filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIEdgePreserveUpsample
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var lumaSigma: Float

A value that specifies the influence of the input image’s luma information on the upsampling operation.

**Required**

var smallImage: CIImage?

The image that the filter upsamples.

**Required**

var spatialSigma: Float

A value that specifies the influence of the input image’s spatial information on the upsampling operation.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func edgePreserveUpsample() -> any CIFilter &amp; CIEdgePreserveUpsample

Creates a high-quality upscaled image.

