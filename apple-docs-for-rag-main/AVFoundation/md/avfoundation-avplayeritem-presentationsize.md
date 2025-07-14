

- AVFoundation
- AVPlayerItem
-  presentationSize 

Instance Property

# presentationSize

The size at which the visual portion of the item is presented by the player.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
nonisolated
var presentationSize: CGSize { get }
```

## Discussion

This property can be accessed at any time, but may return a value of `CGSizeZero` prior to the player item becoming ready to play. You can use key-value observing to obtain the player item’s valid presentation size as early as possible.

## See Also

### Configuring Presentation

var preferredMaximumResolution: CGSize

The desired maximum resolution of a video that is to be downloaded.

var videoApertureMode: AVVideoApertureMode

The video aperture mode to apply during playback.

struct AVVideoApertureMode

A value that describes how a video is scaled or cropped.

