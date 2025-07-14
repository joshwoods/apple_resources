

- AVFoundation
- AVAssetImageGenerator
-  appliesPreferredTrackTransform 

Instance Property

# appliesPreferredTrackTransform

A Boolean value that specifies whether to apply the track matrix or matrices when generating an image from the asset.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var appliesPreferredTrackTransform: Bool { get set }
```

## Discussion

The default value is false. This class only supports rotation by 90, 180, or 270 degrees.

The image generator ignores this property if you set a value for the videoComposition property.

## See Also

### Configuring Image Generation

var maximumSize: CGSize

The maximum size of images to generate.

var requestedTimeToleranceBefore: CMTime

A maximum length of time before the requested time to allow image generation to occur.

var requestedTimeToleranceAfter: CMTime

A maximum length of time after the requested time to allow image generation to occur.

var dynamicRangePolicy: AVAssetImageGenerator.DynamicRangePolicy

The dynamic range policy to use when generating images.

struct DynamicRangePolicy

A type that specifies the dynamic range policy to apply when generating images.

var apertureMode: AVAssetImageGenerator.ApertureMode?

Specifies the aperture mode for the generated image.

struct ApertureMode

Constants that define aperture modes to use when generating images.

