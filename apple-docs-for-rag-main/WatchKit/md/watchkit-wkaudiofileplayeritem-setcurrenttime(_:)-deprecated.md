

- WatchKit
- WKAudioFilePlayerItem
-  setCurrentTime(\_:) Deprecated

Instance Method

# setCurrentTime(\_:)

Sets the playback point, measured in seconds, from the beginning of the audio file.

watchOS 3.2–6.0Deprecated

``` source
func setCurrentTime(_ currentTime: TimeInterval)
```

Deprecated

Use AVFoundation’s AVPlayer and AVQueuePlayer instead

## Parameters 

`currentTime`  

The offset of the current playback position, measured in seconds from the start of the sound.

## Discussion

Use this method to seek a specific point in a sound file or to implement fast-forward and rewind functions.

## See Also

### Managing the Playback Position

var currentTime: TimeInterval

The current playback point, measured in seconds, from the beginning of the audio file.

Deprecated

