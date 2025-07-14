

- AVFAudio
- AVAudioRecorderDelegate
-  audioRecorderEndInterruption(\_:withFlags:) Deprecated

Instance Method

# audioRecorderEndInterruption(\_:withFlags:)

Tells the delegate that the audio session interruption ended with flags.

visionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func audioRecorderEndInterruption(
    _ recorder: AVAudioRecorder,
    withFlags flags: Int
)
```

Deprecated

Observe audio session interruption notifications instead. See Handling audio interruptions for more information.

## Parameters 

`recorder`  

The interrupted audio recorder.

`flags`  

The flags that indicate the state of the audio session.

## See Also

### Responding to Audio Interruptions

func audioRecorderBeginInterruption(AVAudioRecorder)

Tells the delegate that the system interrupted the audio recording.

Deprecated

func audioRecorderEndInterruption(AVAudioRecorder)

Tells the delegate that the audio session interruption ended.

Deprecated

func audioRecorderEndInterruption(AVAudioRecorder, withOptions: Int)

Tells the delegate that the audio session interruption ended with options.

Deprecated

