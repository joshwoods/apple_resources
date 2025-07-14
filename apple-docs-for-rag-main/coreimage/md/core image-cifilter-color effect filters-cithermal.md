

- Core Image
- CIFilter
- Color Effect Filters
-  CIThermal 

Protocol

# CIThermal

The properties you use to configure a thermal filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIThermal
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func thermal() -> any CIFilter &amp; CIThermal

Alters the image to make it look like it was taken by a thermal camera.

