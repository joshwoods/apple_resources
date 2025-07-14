

- AVFoundation
- AVPlayerItem
-  videoApertureMode 

Instance Property

# videoApertureMode

The video aperture mode to apply during playback.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
nonisolated
var videoApertureMode: AVVideoApertureMode { get set }
```

## Discussion

The default value for this property is cleanAperture.

## See Also

### Configuring Presentation

var presentationSize: CGSize

The size at which the visual portion of the item is presented by the player.

var preferredMaximumResolution: CGSize

The desired maximum resolution of a video that is to be downloaded.

struct AVVideoApertureMode

A value that describes how a video is scaled or cropped.

