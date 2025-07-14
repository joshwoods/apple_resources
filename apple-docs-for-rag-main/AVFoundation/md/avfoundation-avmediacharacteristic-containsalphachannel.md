

- AVFoundation
- AVMediaCharacteristic
-  containsAlphaChannel 

Type Property

# containsAlphaChannel

A media characteristic that indicates that a track contains an alpha channel.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
static let containsAlphaChannel: AVMediaCharacteristic
```

## Discussion

To determine whether the alpha is straight or pre-multiplied, look for a format description extension with key kCMFormatDescriptionExtension_AlphaChannelMode.

## See Also

### Visual

static let visual: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes visual content.

static let containsHDRVideo: AVMediaCharacteristic

A media characteristic that indicates that a track contains HDR video.

static let frameBased: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes frame-based content.

static let usesWideGamutColorSpace: AVMediaCharacteristic

A media characteristic that indicates that a track uses a wide-gamut color space.

static let containsStereoMultiviewVideo: AVMediaCharacteristic

A media characteristic that indicates that a track contains stereoscopic video captured in a multiview compression format.

static let carriesVideoStereoMetadata: AVMediaCharacteristic

A media characteristic that indicates that the stereoscopic video track carries additional information related to the stereoscopic video.

static let indicatesHorizontalFieldOfView: AVMediaCharacteristic

A media characteristic that indicates the video track carries information related to the horizontal field of view.

