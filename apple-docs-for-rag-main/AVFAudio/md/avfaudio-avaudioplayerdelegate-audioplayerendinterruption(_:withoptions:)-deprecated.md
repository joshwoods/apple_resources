

- AVFAudio
- AVAudioPlayerDelegate
-  audioPlayerEndInterruption(\_:withOptions:) Deprecated

Instance Method

# audioPlayerEndInterruption(\_:withOptions:)

Tells the delegate when the audio session interruption ends with options.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func audioPlayerEndInterruption(
    _ player: AVAudioPlayer,
    withOptions flags: Int
)
```

Deprecated

Observe audio session interruption notifications instead. See Handling audio interruptions for more information.

## Parameters 

`player`  

The audio player with the interruption that ends.

`flags`  

The options that indicate the state of the audio session.

## See Also

### Responding to Audio Interruptions

func audioPlayerBeginInterruption(AVAudioPlayer)

Tells the delegate when the system interrupts the audio player’s playback.

Deprecated

func audioPlayerEndInterruption(AVAudioPlayer)

Tells the delegate when the audio session interruption ends.

Deprecated

func audioPlayerEndInterruption(AVAudioPlayer, withFlags: Int)

Tells the delegate when the audio session interruption ends with flags.

Deprecated

