

- WatchKit
- WKAudioFilePlayer
-  currentTime Deprecated

Instance Property

# currentTime

The elapsed time for the current playing item.

watchOS 2.0–6.0Deprecated

``` source
var currentTime: TimeInterval { get }
```

## Discussion

This property refers to how much of the audio file has already been played. The value in this property is updated during playback to reflect the current position of the playhead.

The value of this property is valid only when the player item’s status is WKAudioFilePlayerStatus.readyToPlay.

