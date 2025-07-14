

- Media Player
- MPMoviePlayerController
-  duration Deprecated

Instance Property

# duration

The duration of the movie, measured in seconds.

iOS 3.2–9.0DeprecatediPadOS 3.2–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
var duration: TimeInterval { get }
```

Deprecated

Use AVPlayerViewController in AVKit

## Discussion

If the duration of the movie is not known, the value in this property is `0.0`. If the duration is subsequently determined, this property is updated and a MPMovieDurationAvailableNotification notification is posted.

## See Also

### Accessing the movie duration

var playableDuration: TimeInterval

The amount of currently playable content.

Deprecated

