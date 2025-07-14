

- AVFAudio
- AVAudioRecorderDelegate
-  audioRecorderBeginInterruption(\_:) Deprecated

Instance Method

# audioRecorderBeginInterruption(\_:)

Tells the delegate that the system interrupted the audio recording.

iOS 2.2–8.0DeprecatediPadOS 2.2–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func audioRecorderBeginInterruption(_ recorder: AVAudioRecorder)
```

Deprecated

Observe audio session interruption notifications instead. See Handling audio interruptions for more information.

## Parameters 

`recorder`  

The interrupted audio recorder.

## See Also

### Responding to Audio Interruptions

func audioRecorderEndInterruption(AVAudioRecorder)

Tells the delegate that the audio session interruption ended.

Deprecated

func audioRecorderEndInterruption(AVAudioRecorder, withOptions: Int)

Tells the delegate that the audio session interruption ended with options.

Deprecated

func audioRecorderEndInterruption(AVAudioRecorder, withFlags: Int)

Tells the delegate that the audio session interruption ended with flags.

Deprecated

