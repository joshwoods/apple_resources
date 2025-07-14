

- Core Image
- CIFilter
- Stylizing Filters
-  CIHighlightShadowAdjust 

Protocol

# CIHighlightShadowAdjust

The properties you use to configure a highlight-shadow adjust filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIHighlightShadowAdjust
```

## Topics

### Instance Properties

var highlightAmount: Float

The amount of adjustment to the highlights in the image.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The shadow highlight radius.

**Required**

var shadowAmount: Float

The amount of adjustment to the shadows in the image.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func highlightShadowAdjust() -> any CIFilter &amp; CIHighlightShadowAdjust

Adjusts the highlights of colors to reduce shadows.

