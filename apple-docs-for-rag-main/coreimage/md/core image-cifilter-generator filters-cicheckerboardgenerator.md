

- Core Image
- CIFilter
- Generator Filters
-  CICheckerboardGenerator 

Protocol

# CICheckerboardGenerator

The properties you use to configure a checkerboard generator filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CICheckerboardGenerator
```

## Topics

### Instance Properties

var center: CGPoint

The center of the effect as x and y coordinates.

**Required**

var color0: CIColor

A color to use for the first set of squares.

**Required**

var color1: CIColor

A color to use for the second set of squares.

**Required**

var sharpness: Float

The sharpness of the edges in the pattern.

**Required**

var width: Float

The width of the squares in the pattern.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func checkerboardGenerator() -> any CIFilter &amp; CICheckerboardGenerator

Generates a checkerboard image.

