

- AVFoundation
- AVAssetImageGenerator
-  maximumSize 

Instance Property

# maximumSize

The maximum size of images to generate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var maximumSize: CGSize { get set }
```

## Mentioned in 

Creating images from a video asset

## Discussion

The default value is zero, which generates images at the asset’s unscaled dimensions.

Setting a size scales images to fit their defined bounding boxes. You define the aspect ratio of the scaled image by setting a value for the apertureMode property.

## See Also

### Configuring Image Generation

var requestedTimeToleranceBefore: CMTime

A maximum length of time before the requested time to allow image generation to occur.

var requestedTimeToleranceAfter: CMTime

A maximum length of time after the requested time to allow image generation to occur.

var dynamicRangePolicy: AVAssetImageGenerator.DynamicRangePolicy

The dynamic range policy to use when generating images.

struct DynamicRangePolicy

A type that specifies the dynamic range policy to apply when generating images.

var appliesPreferredTrackTransform: Bool

A Boolean value that specifies whether to apply the track matrix or matrices when generating an image from the asset.

var apertureMode: AVAssetImageGenerator.ApertureMode?

Specifies the aperture mode for the generated image.

struct ApertureMode

Constants that define aperture modes to use when generating images.

