

- Core Image
- CIFilter
- Color Effect Filters
-  CILabDeltaE 

Protocol

# CILabDeltaE

The properties you use to configure a Lab Delta E filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CILabDeltaE
```

## Topics

### Instance Properties

var image2: CIImage?

The second input image for comparison.

**Required**

var inputImage: CIImage?

The first input image for comparison.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func labDeltaE() -> any CIFilter &amp; CILabDeltaE

Compares an image’s color values.

