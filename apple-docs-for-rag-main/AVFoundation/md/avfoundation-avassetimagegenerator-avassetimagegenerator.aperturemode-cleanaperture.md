

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.ApertureMode
-  cleanAperture 

Type Property

# cleanAperture

A mode that applies both pixel aspect ratio and clean aperture.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
static let cleanAperture: AVAssetImageGenerator.ApertureMode
```

## Discussion

An image’s clean aperture is a region of video free from transition artifacts caused by the encoding of the signal.

## See Also

### Aperture Modes

static let encodedPixels: AVAssetImageGenerator.ApertureMode

A mode that applies neither pixel aspect ratio nor clean aperture.

static let productionAperture: AVAssetImageGenerator.ApertureMode

A mode that applies only pixel aspect ratio.

