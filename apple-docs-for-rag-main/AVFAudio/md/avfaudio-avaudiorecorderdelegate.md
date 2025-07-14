

- AVFAudio
-  AVAudioRecorderDelegate 

Protocol

# AVAudioRecorderDelegate

A protocol that defines the methods to respond to audio recording events and encoding errors.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
protocol AVAudioRecorderDelegate : NSObjectProtocol, Sendable
```

## Topics

### Responding to Recording Completion

func audioRecorderDidFinishRecording(AVAudioRecorder, successfully: Bool)

Tells the delegate when recording stops or finishes due to reaching its time limit.

### Responding to Audio Encoding Errors

func audioRecorderEncodeErrorDidOccur(AVAudioRecorder, error: (any Error)?)

Tells the delegate that the audio recorder encountered an encoding error during recording.

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

func audioRecorderEndInterruption(AVAudioRecorder, withFlags: Int)

Tells the delegate that the audio session interruption ended with flags.

Deprecated

## Relationships

### Inherits From

- NSObjectProtocol
- Sendable

## See Also

### Responding to recorder events

var delegate: (any AVAudioRecorderDelegate)?

The delegate object for the audio recorder.

