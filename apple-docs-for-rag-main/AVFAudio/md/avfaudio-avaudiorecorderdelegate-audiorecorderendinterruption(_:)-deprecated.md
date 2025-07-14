

- AVFAudio
- AVAudioRecorderDelegate
-  audioRecorderEndInterruption(\_:) Deprecated

Instance Method

# audioRecorderEndInterruption(\_:)

Tells the delegate that the audio session interruption ended.

visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func audioRecorderEndInterruption(_ recorder: AVAudioRecorder)
```

Deprecated

Observe audio session interruption notifications instead. See Handling audio interruptions for more information.

## Parameters 

`recorder`  

The interrupted audio recorder.

## See Also

### Responding to Audio Interruptions

func audioRecorderBeginInterruption(AVAudioRecorder)

Tells the delegate that the system interrupted the audio recording.

Deprecated

func audioRecorderEndInterruption(AVAudioRecorder, withOptions: Int)

Tells the delegate that the audio session interruption ended with options.

Deprecated

func audioRecorderEndInterruption(AVAudioRecorder, withFlags: Int)

Tells the delegate that the audio session interruption ended with flags.

Deprecated

