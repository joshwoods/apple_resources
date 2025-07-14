

- Core Image
- CIFilter
- Sharpening Filters
-  CISharpenLuminance 

Protocol

# CISharpenLuminance

The properties you use to configure a sharpen luminance filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CISharpenLuminance
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The distance from the center of the effect.

**Required**

var sharpness: Float

The amount of sharpening to apply.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func sharpenLuminance() -> any CIFilter &amp; CISharpenLuminance

Applies a sharpening effect to an image.

