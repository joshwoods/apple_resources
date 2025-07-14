

- WatchKit
- WKAudioFilePlayer
-  error Deprecated

Instance Property

# error

An error that describes the cause of a failure.

watchOS 2.0–6.0Deprecated

``` source
var error: (any Error)? { get }
```

## Discussion

This property is `nil` unless the status property of the player item is WKAudioFilePlayerStatus.failed. When playback fails, the error indicates the reason for the failure.

## See Also

### Getting Information About the Player

var currentItem: WKAudioFilePlayerItem?

The player’s current item.

Deprecated

var status: WKAudioFilePlayerStatus

The status of the player.

Deprecated

