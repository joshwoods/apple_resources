

- WatchKit
- WKAudioFilePlayer
-  status Deprecated

Instance Property

# status

The status of the player.

watchOS 2.0–6.0Deprecated

``` source
var status: WKAudioFilePlayerStatus { get }
```

## Discussion

When the value of this property is WKAudioFilePlayerStatus.failed, the error property contains the reason for the failure.

## See Also

### Getting Information About the Player

var currentItem: WKAudioFilePlayerItem?

The player’s current item.

Deprecated

var error: (any Error)?

An error that describes the cause of a failure.

Deprecated

