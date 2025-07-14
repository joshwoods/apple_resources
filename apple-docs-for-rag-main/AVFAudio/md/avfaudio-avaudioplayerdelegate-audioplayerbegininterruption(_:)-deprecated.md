

- AVFAudio
- AVAudioPlayerDelegate
-  audioPlayerBeginInterruption(\_:) Deprecated

Instance Method

# audioPlayerBeginInterruption(\_:)

Tells the delegate when the system interrupts the audio player’s playback.

iOS 2.2–8.0DeprecatediPadOS 2.2–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOSvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func audioPlayerBeginInterruption(_ player: AVAudioPlayer)
```

Deprecated

Observe audio session interruption notifications instead. See Handling audio interruptions for more information.

## Parameters 

`player`  

The interrupted audio player.

## See Also

### Responding to Audio Interruptions

func audioPlayerEndInterruption(AVAudioPlayer)

Tells the delegate when the audio session interruption ends.

Deprecated

func audioPlayerEndInterruption(AVAudioPlayer, withOptions: Int)

Tells the delegate when the audio session interruption ends with options.

Deprecated

func audioPlayerEndInterruption(AVAudioPlayer, withFlags: Int)

Tells the delegate when the audio session interruption ends with flags.

Deprecated

