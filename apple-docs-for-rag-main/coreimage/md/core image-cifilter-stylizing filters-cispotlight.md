

- Core Image
- CIFilter
- Stylizing Filters
-  CISpotLight 

Protocol

# CISpotLight

The properties you use to configure a spotlight filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CISpotLight
```

## Topics

### Instance Properties

var brightness: Float

The brightness of the spotlight.

**Required**

var color: CIColor

The color of the spotlight.

**Required**

var concentration: Float

The size of the spotlight.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var lightPointsAt: CIVector

The x and y position that the spotlight points at.

**Required**

var lightPosition: CIVector

The x and y position of the spotlight.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func spotLight() -> any CIFilter &amp; CISpotLight

Highlights a definined area of the image.

