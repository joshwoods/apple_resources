

- AVFAudio
- AVAudioRecorderDelegate
-  audioRecorderEndInterruption(\_:withOptions:) Deprecated

Instance Method

# audioRecorderEndInterruption(\_:withOptions:)

Tells the delegate that the audio session interruption ended with options.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func audioRecorderEndInterruption(
    _ recorder: AVAudioRecorder,
    withOptions flags: Int
)
```

Deprecated

Observe audio session interruption notifications instead. See Handling audio interruptions for more information.

## Parameters 

`recorder`  

The interrupted audio recorder.

`flags`  

The options that indicate the state of the audio session.

## See Also

### Responding to Audio Interruptions

func audioRecorderBeginInterruption(AVAudioRecorder)

Tells the delegate that the system interrupted the audio recording.

Deprecated

func audioRecorderEndInterruption(AVAudioRecorder)

Tells the delegate that the audio session interruption ended.

Deprecated

func audioRecorderEndInterruption(AVAudioRecorder, withFlags: Int)

Tells the delegate that the audio session interruption ended with flags.

Deprecated

