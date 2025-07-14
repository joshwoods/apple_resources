

- Core Image
- CIFilter
- Color Adjustment Filters
-  CIColorControls 

Protocol

# CIColorControls

The properties you use to configure a color controls filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIColorControls
```

## Topics

### Instance Properties

var brightness: Float

The amount of brightness to apply.

**Required**

var contrast: Float

The amount of contrast to apply.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var saturation: Float

The amount of saturation to apply.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func colorControls() -> any CIFilter &amp; CIColorControls

Alters the brightness, contrast, and saturation of an image’s colors.

