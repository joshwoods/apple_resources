

- Core Image
- CIFilter
- Stylizing Filters
-  CISpotColor 

Protocol

# CISpotColor

The properties you use to configure a spot color filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CISpotColor
```

## Topics

### Instance Properties

var centerColor1: CIColor

The center value of the first color range to replace.

**Required**

var centerColor2: CIColor

The center value of the second color range to replace.

**Required**

var centerColor3: CIColor

The center value of the third color range to replace.

**Required**

var closeness1: Float

A value that indicates how closely the first color must match before it’s replaced.

**Required**

var closeness2: Float

A value that indicates how closely the second color must match before it’s replaced.

**Required**

var closeness3: Float

A value that indicates how closely the third color must match before it’s replaced.

**Required**

var contrast1: Float

The contrast of the first replacement color.

**Required**

var contrast2: Float

The contrast of the second replacement color.

**Required**

var contrast3: Float

The contrast of the third replacement color.

**Required**

var inputImage: CIImage?

The image to use as an input image.

**Required**

var replacementColor1: CIColor

A replacement color for the first color range.

**Required**

var replacementColor2: CIColor

A replacement color for the second color range.

**Required**

var replacementColor3: CIColor

A replacement color for the third color range.

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func spotColor() -> any CIFilter &amp; CISpotColor

Replaces colors of an image with specifed colors.

