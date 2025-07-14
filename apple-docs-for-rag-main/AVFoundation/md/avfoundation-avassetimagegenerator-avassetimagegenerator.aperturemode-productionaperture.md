

- AVFoundation
- AVAssetImageGenerator
- AVAssetImageGenerator.ApertureMode
-  productionAperture 

Type Property

# productionAperture

A mode that applies only pixel aspect ratio.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
static let productionAperture: AVAssetImageGenerator.ApertureMode
```

## Discussion

The image isn’t cropped to the clean aperture region, but it’s scaled according to the pixel aspect ratio. Use this option when you want to see all the pixels in your video, including the edges.

## See Also

### Aperture Modes

static let cleanAperture: AVAssetImageGenerator.ApertureMode

A mode that applies both pixel aspect ratio and clean aperture.

static let encodedPixels: AVAssetImageGenerator.ApertureMode

A mode that applies neither pixel aspect ratio nor clean aperture.

