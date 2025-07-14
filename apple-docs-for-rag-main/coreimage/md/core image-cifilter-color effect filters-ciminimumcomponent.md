

- Core Image
- CIFilter
- Color Effect Filters
-  CIMinimumComponent 

Protocol

# CIMinimumComponent

The properties you use to configure a minimum component filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIMinimumComponent
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

class func minimumComponent() -> any CIFilter &amp; CIMinimumComponent

Creates a minimum RGB grayscale image.

