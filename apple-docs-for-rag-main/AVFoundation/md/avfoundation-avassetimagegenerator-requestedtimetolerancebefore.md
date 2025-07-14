

- AVFoundation
- AVAssetImageGenerator
-  requestedTimeToleranceBefore 

Instance Property

# requestedTimeToleranceBefore

A maximum length of time before the requested time to allow image generation to occur.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var requestedTimeToleranceBefore: CMTime { get set }
```

## Mentioned in 

Creating images from a video asset

## Discussion

The default value is positiveInfinity. Set the values of requestedTimeToleranceBefore and requestedTimeToleranceAfter to zero to request frame-accurate image generation; this may incur additional decoding delay.

## See Also

### Configuring Image Generation

var maximumSize: CGSize

The maximum size of images to generate.

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

