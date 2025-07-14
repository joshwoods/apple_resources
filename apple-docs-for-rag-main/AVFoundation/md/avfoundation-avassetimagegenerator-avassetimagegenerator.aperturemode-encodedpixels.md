

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.ApertureMode
-  encodedPixels 

Type Property

# encodedPixels

A mode that applies neither pixel aspect ratio nor clean aperture.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
static let encodedPixels: AVAssetImageGenerator.ApertureMode
```

## Discussion

The image isn’t cropped to the clean aperture region and isn’t scaled according to the pixel aspect ratio. It displays the image according to its encoded dimensions.

## See Also

### Aperture Modes

static let cleanAperture: AVAssetImageGenerator.ApertureMode

A mode that applies both pixel aspect ratio and clean aperture.

static let productionAperture: AVAssetImageGenerator.ApertureMode

A mode that applies only pixel aspect ratio.

