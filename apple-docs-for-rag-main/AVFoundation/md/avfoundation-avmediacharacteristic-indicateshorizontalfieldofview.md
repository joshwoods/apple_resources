

- AVFoundation
- AVMediaCharacteristic
-  indicatesHorizontalFieldOfView 

Type Property

# indicatesHorizontalFieldOfView

A media characteristic that indicates the video track carries information related to the horizontal field of view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
static let indicatesHorizontalFieldOfView: AVMediaCharacteristic
```

## Discussion

This media characteristic is present when the CMVideoFormatDescription includes a kCMFormatDescriptionExtension_HorizontalFieldOfView extension. This is not an indication that the field of view is expanded beyond or more narrow than typical horizontal fields of view.

The value of this characteristic is `public.indicates-horizontal-field-of-view`.

Note

The presence of this characteristic is strictly inferred from the format description of the associated track.

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

static let usesWideGamutColorSpace: AVMediaCharacteristic

A media characteristic that indicates that a track uses a wide-gamut color space.

static let containsStereoMultiviewVideo: AVMediaCharacteristic

A media characteristic that indicates that a track contains stereoscopic video captured in a multiview compression format.

static let carriesVideoStereoMetadata: AVMediaCharacteristic

A media characteristic that indicates that the stereoscopic video track carries additional information related to the stereoscopic video.

