

- AVFoundation
- AVAssetImageGenerator
-  AVAssetImageGenerator.ApertureMode 

Structure

# AVAssetImageGenerator.ApertureMode

Constants that define aperture modes to use when generating images.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
struct ApertureMode
```

## Topics

### Aperture Modes

static let cleanAperture: AVAssetImageGenerator.ApertureMode

A mode that applies both pixel aspect ratio and clean aperture.

static let encodedPixels: AVAssetImageGenerator.ApertureMode

A mode that applies neither pixel aspect ratio nor clean aperture.

static let productionAperture: AVAssetImageGenerator.ApertureMode

A mode that applies only pixel aspect ratio.

### Initializers

init(rawValue: String)

Creates an aperture mode with a string value.

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

struct DynamicRangePolicy

A type that specifies the dynamic range policy to apply when generating images.

var appliesPreferredTrackTransform: Bool

A Boolean value that specifies whether to apply the track matrix or matrices when generating an image from the asset.

var apertureMode: AVAssetImageGenerator.ApertureMode?

Specifies the aperture mode for the generated image.

