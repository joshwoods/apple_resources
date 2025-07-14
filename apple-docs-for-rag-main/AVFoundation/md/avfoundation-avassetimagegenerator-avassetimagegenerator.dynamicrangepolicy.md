

- AVFoundation
- AVAssetImageGenerator
-  AVAssetImageGenerator.DynamicRangePolicy 

Structure

# AVAssetImageGenerator.DynamicRangePolicy

A type that specifies the dynamic range policy to apply when generating images.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
struct DynamicRangePolicy
```

## Topics

### Policies

static let forceSDR: AVAssetImageGenerator.DynamicRangePolicy

A policy that forces conversion to standard dynamic range.

static let matchSource: AVAssetImageGenerator.DynamicRangePolicy

A policy that preserves the color parameters of the source media.

### Initializers

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var appliesPreferredTrackTransform: Bool

A Boolean value that specifies whether to apply the track matrix or matrices when generating an image from the asset.

var apertureMode: AVAssetImageGenerator.ApertureMode?

Specifies the aperture mode for the generated image.

struct ApertureMode

Constants that define aperture modes to use when generating images.

