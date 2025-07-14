

- AVFoundation
- AVMediaCharacteristic
-  containsHDRVideo 

Type Property

# containsHDRVideo

A media characteristic that indicates that a track contains HDR video.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
static let containsHDRVideo: AVMediaCharacteristic
```

## Discussion

HDR video contains extended dynamic range that requires explicit support when compositing. The system infers this characteristic from the format description of the associated track.

The value of this characteristic is `public.contains-hdr-video`.

## See Also

### Visual

static let visual: AVMediaCharacteristic

A media characteristic that indicates that a track or media selection option includes visual content.

static let containsAlphaChannel: AVMediaCharacteristic

A media characteristic that indicates that a track contains an alpha channel.

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

