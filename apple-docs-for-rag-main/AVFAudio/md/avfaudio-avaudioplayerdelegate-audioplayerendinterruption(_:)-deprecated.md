

- AVFAudio
- AVAudioPlayerDelegate
-  audioPlayerEndInterruption(\_:) Deprecated

Instance Method

# audioPlayerEndInterruption(\_:)

Tells the delegate when the audio session interruption ends.

tvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func audioPlayerEndInterruption(_ player: AVAudioPlayer)
```

Deprecated

Observe audio session interruption notifications instead. See Handling audio interruptions for more information.

## Parameters 

`player`  

The audio player with the interruption that ends.

## See Also

### Responding to Audio Interruptions

func audioPlayerBeginInterruption(AVAudioPlayer)

Tells the delegate when the system interrupts the audio player’s playback.

Deprecated

func audioPlayerEndInterruption(AVAudioPlayer, withOptions: Int)

Tells the delegate when the audio session interruption ends with options.

Deprecated

func audioPlayerEndInterruption(AVAudioPlayer, withFlags: Int)

Tells the delegate when the audio session interruption ends with flags.

Deprecated

