

- AVFoundation
- AVMediaCharacteristic
-  usesWideGamutColorSpace 

Type Property

# usesWideGamutColorSpace

A media characteristic that indicates that a track uses a wide-gamut color space.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
static let usesWideGamutColorSpace: AVMediaCharacteristic
```

## Mentioned in 

Tagging Media with Video Color Information

## Discussion

Tracks that use a wide-gamut color space may use colors that can’t be accurately represented in standard RGB mode.

## See Also

### Visual

static let visual: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes visual content.

static let containsAlphaChannel: AVMediaCharacteristic

A media characteristic that indicates that a track contains an alpha channel.

static let containsHDRVideo: AVMediaCharacteristic

A media characteristic that indicates that a track contains HDR video.

static let frameBased: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes frame-based content.

static let containsStereoMultiviewVideo: AVMediaCharacteristic

A media characteristic that indicates that a track contains stereoscopic video captured in a multiview compression format.

static let carriesVideoStereoMetadata: AVMediaCharacteristic

A media characteristic that indicates that the stereoscopic video track carries additional information related to the stereoscopic video.

static let indicatesHorizontalFieldOfView: AVMediaCharacteristic

A media characteristic that indicates the video track carries information related to the horizontal field of view.

