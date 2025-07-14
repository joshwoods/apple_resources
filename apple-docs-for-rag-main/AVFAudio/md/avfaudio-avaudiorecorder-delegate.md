

- AVFAudio
- AVAudioRecorder
-  delegate 

Instance Property

# delegate

The delegate object for the audio recorder.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+macOS 10.7+tvOS 17.0+visionOS 1.0+watchOS 4.0+

``` source
weak var delegate: (any AVAudioRecorderDelegate)? { get set }
```

## See Also

### Responding to recorder events

protocol AVAudioRecorderDelegate

A protocol that defines the methods to respond to audio recording events and encoding errors.

