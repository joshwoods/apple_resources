

- Core Image
- CIFilter
- Color Effect Filters
-  CIPhotoEffect 

Protocol

# CIPhotoEffect

The properties you use to configure a photo-effect filter.

iOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
protocol CIPhotoEffect
```

## Topics

### Instance Properties

var inputImage: CIImage?

The image to use as an input image.

**Required**

var extrapolate: Bool

**Required**

## Relationships

### Inherits From

- CIFilterProtocol

## See Also

### Related Documentation

class func photoEffectChrome() -> any CIFilter &amp; CIPhotoEffect

Exaggerates an image’s colors.

class func photoEffectFade() -> any CIFilter &amp; CIPhotoEffect

Diminishes an image’s colors.

class func photoEffectInstant() -> any CIFilter &amp; CIPhotoEffect

Desaturates an image’s colors.

class func photoEffectMono() -> any CIFilter &amp; CIPhotoEffect

Adjust an image’s colors to black and white.

class func photoEffectNoir() -> any CIFilter &amp; CIPhotoEffect

Adjusts an image’s colors to black and white and intensifies the contrast.

class func photoEffectProcess() -> any CIFilter &amp; CIPhotoEffect

Lowers the contrast of the input image.

class func photoEffectTonal() -> any CIFilter &amp; CIPhotoEffect

Adjusts an image’s colors to black and white.

class func photoEffectTransfer() -> any CIFilter &amp; CIPhotoEffect

Brightens an image’s colors.

