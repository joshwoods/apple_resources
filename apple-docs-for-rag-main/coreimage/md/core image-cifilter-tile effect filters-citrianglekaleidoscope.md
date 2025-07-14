

- Core Image
- CIFilter
- Tile Effect Filters
-  CITriangleKaleidoscope 

Protocol

# CITriangleKaleidoscope

The properties you use to configure a triangle kaleidoscope filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CITriangleKaleidoscope
```

## Topics

### Instance Properties

var decay: Float

A value that determines how fast the color fades from the center triangle.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var point: CGPoint

The x and y position to use as the center of the triangular area in the input image.

**Required**

var rotation: Float

The rotation angle of the triangle.

**Required**

var size: Float

The size, in pixels, of the triangle.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func triangleKaleidoscope() -> any CIFilter &amp; CITriangleKaleidoscope

Create a triangular kaleidoscope effect and then tiles the result.

