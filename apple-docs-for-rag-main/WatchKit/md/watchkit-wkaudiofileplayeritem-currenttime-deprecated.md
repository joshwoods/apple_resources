

- WatchKit
- WKAudioFilePlayerItem
-  currentTime Deprecated

Instance Property

# currentTime

The current playback point, measured in seconds, from the beginning of the audio file.

watchOS 2.0–6.0Deprecated

``` source
var currentTime: TimeInterval { get }
```

## Discussion

This property refers to how much of the audio file has already been played. The value in this property is updated during playback to reflect the current position of the playhead.

The value of this property is valid only when the player item’s status is WKAudioFilePlayerItemStatus.readyToPlay.

## See Also

### Managing the Playback Position

func setCurrentTime(TimeInterval)

Sets the playback point, measured in seconds, from the beginning of the audio file.

Deprecated

