

- AVKit
- AVPlayerViewController
-  exitsFullScreenWhenPlaybackEnds 

Instance Property

# exitsFullScreenWhenPlaybackEnds

A Boolean value that indicates whether the player exits full-screen mode when playback ends.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var exitsFullScreenWhenPlaybackEnds: Bool { get set }
```

## Discussion

If you enqueue multiple player items, the player exits full-screen mode after it plays all remaining items in the queue.

The default value is false.

## See Also

### Managing Full-Screen Behavior

var entersFullScreenWhenPlaybackBegins: Bool

A Boolean value that determines whether the player automatically displays in full screen when the user taps the play button.

