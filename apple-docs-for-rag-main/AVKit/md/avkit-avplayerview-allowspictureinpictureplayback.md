

- AVKit
- AVPlayerView
-  allowsPictureInPicturePlayback 

Instance Property

# allowsPictureInPicturePlayback

A Boolean value that determines whether the player view allows Picture in Picture playback.

macOS 10.15+

``` source
@MainActor
var allowsPictureInPicturePlayback: Bool { get set }
```

## Discussion

The default value is false.

## See Also

### Configuring Picture in Picture

var pictureInPictureDelegate: (any AVPlayerViewPictureInPictureDelegate)?

The Picture in Picture delegate object.

protocol AVPlayerViewPictureInPictureDelegate

A protocol that defines the methods to implement to respond to Picture in Picture playback events.

