

- Core Image
- CIFilter
- Stylizing Filters
-  CIDepthOfField 

Protocol

# CIDepthOfField

The properties you use to configure a depth-of-field filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIDepthOfField
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var point0: CGPoint

The first point in the focused region of the output image.

**Required**

var point1: CGPoint

The second point in the focused region of the output image.

**Required**

var radius: Float

The distance from the center of the effect.

**Required**

var saturation: Float

The amount to adjust the saturation by.

**Required**

var unsharpMaskIntensity: Float

The intensity of the unsharp mask effect applied to the in-focus area.

**Required**

var unsharpMaskRadius: Float

The radius of the unsharp mask effect applied to the in-focus area.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func depthOfField() -> any CIFilter &amp; CIDepthOfField

Simulates a depth of field effect.

