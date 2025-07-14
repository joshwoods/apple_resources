

- Core Image
- CIFilter
- Tile Effect Filters
-  CIKaleidoscope 

Protocol

# CIKaleidoscope

The properties you use to configure a kaleidoscope filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIKaleidoscope
```

## Topics

### Instance Properties

var angle: Float

The angle of the reflection.

**Required**

var center: CGPoint

The x and y position to use as the center of the effect.

**Required**

var count: Int

The number of reflections in the pattern.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func kaleidoscope() -> any CIFilter &amp; CIKaleidoscope

Creates a 12-way kaleidoscopic image from an image.

