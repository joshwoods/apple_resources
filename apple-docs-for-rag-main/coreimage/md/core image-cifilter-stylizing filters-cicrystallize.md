

- Core Image
- CIFilter
- Stylizing Filters
-  CICrystallize 

Protocol

# CICrystallize

The properties you use to configure a crystalize filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CICrystallize
```

## Topics

### Instance Properties

var center: CGPoint

The center of the effect as x and y coordinates.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The radius, in pixels, of the effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func crystallize() -> any CIFilter &amp; CICrystallize

Creates an image made with a series of colorful polygons.

