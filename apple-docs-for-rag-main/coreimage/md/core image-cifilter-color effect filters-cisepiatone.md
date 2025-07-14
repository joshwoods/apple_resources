

- Core Image
- CIFilter
- Color Effect Filters
-  CISepiaTone 

Protocol

# CISepiaTone

The properties you use to configure a sepia-tone filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CISepiaTone
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var intensity: Float

The intensity of the sepia effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func sepiaTone() -> any CIFilter &amp; CISepiaTone

Adjusts an image’s colors to shades of brown.

