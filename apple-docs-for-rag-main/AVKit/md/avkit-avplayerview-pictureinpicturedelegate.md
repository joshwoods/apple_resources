

- AVKit
- AVPlayerView
-  pictureInPictureDelegate 

Instance Property

# pictureInPictureDelegate

The Picture in Picture delegate object.

macOS 10.15+

``` source
@MainActor
weak var pictureInPictureDelegate: (any AVPlayerViewPictureInPictureDelegate)? { get set }
```

## See Also

### Configuring Picture in Picture

var allowsPictureInPicturePlayback: Bool

A Boolean value that determines whether the player view allows Picture in Picture playback.

protocol AVPlayerViewPictureInPictureDelegate

A protocol that defines the methods to implement to respond to Picture in Picture playback events.

