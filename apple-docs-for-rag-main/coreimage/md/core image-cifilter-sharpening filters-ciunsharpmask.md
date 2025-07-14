

- Core Image
- CIFilter
- Sharpening Filters
-  CIUnsharpMask 

Protocol

# CIUnsharpMask

The properties you use to configure an unsharp mask filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIUnsharpMask
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var intensity: Float

The intensity of the effect.

**Required**

var radius: Float

The radius of the unsharp mask effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func unsharpMask() -> any CIFilter &amp; CIUnsharpMask

Increases an image’s contrast between two colors.

