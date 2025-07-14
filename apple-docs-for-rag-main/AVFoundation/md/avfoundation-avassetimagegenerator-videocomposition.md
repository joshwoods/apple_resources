

- AVFoundation
- AVAssetImageGenerator
-  videoComposition 

Instance Property

# videoComposition

A video composition to use when extracting images from assets with multiple video tracks.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
@NSCopying
var videoComposition: AVVideoComposition? { get set }
```

## Discussion

If you don’t specify a video composition, the generator only uses the first enabled video track.

If specify a video composition, the image generator ignores the value of the appliesPreferredTrackTransform property.

Setting a video composition with any of the following attributes generates an exception:

- A renderScale not equal to `1.0`.

- A renderSize with a width or height less than `0`.

- A frameDuration that’s invalid, or less than or equal to zero.

- A sourceTrackIDForFrameTiming less than zero.

## See Also

### Configuring Compositing

var customVideoCompositor: (any AVVideoCompositing)?

A custom video compositor to use when extracting images from assets with multiple video tracks.

