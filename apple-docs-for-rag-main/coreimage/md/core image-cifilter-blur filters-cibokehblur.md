

- Core Image
- CIFilter
- Blur Filters
-  CIBokehBlur 

Protocol

# CIBokehBlur

The properties you use to configure a bokeh blur filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIBokehBlur
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var radius: Float

The radius of the blur, in pixels.

**Required**

var ringAmount: Float

The amount of extra emphasis at the ring of the bokeh.

**Required**

var ringSize: Float

The radius of the extra emphasis at the ring of the bokeh.

**Required**

var softness: Float

The softness of the bokeh effect.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func bokehBlur() -> any CIFilter &amp; CIBokehBlur

Applies a bokeh effect to an image.

