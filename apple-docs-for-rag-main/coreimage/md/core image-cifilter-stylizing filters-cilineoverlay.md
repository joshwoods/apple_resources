

- Core Image
- CIFilter
- Stylizing Filters
-  CILineOverlay 

Protocol

# CILineOverlay

The properties you use to configure a line overlay filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CILineOverlay
```

## Topics

### Instance Properties

var nrNoiseLevel: Float

The noise level of the image, used with camera data, that's removed before tracing the edges of the image.

**Required**

var nrSharpness: Float

The amount of sharpening done when removing noise in the image before tracing the edges of the image.

**Required**

var contrast: Float

The amount of antialiasing to use on the edges produced by this filter.

**Required**

var edgeIntensity: Float

The accentuation factor of the Sobel gradient information when tracing the edges of the image.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var threshold: Float

A value that determines edge visibility.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func lineOverlay() -> any CIFilter &amp; CILineOverlay

Creates an image that resembles a sketch of the outlines of objects.

