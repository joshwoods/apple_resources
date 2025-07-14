

- Core Image
- CIFilter
- Blur Filters
-  CIMotionBlur 

Protocol

# CIMotionBlur

The properties you use to configure a motion blur filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIMotionBlur
```

## Topics

### Instance Properties

var angle: Float

The angle of the motion, in radians, that determines which direction the blur smears.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The radius of the blur, in pixels.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func motionBlur() -> any CIFilter &amp; CIMotionBlur

Creates motion blur on an image.

