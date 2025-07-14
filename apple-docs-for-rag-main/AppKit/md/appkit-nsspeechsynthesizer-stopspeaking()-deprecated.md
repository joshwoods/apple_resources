

- AppKit
- NSSpeechSynthesizer
-  stopSpeaking() Deprecated

Instance Method

# stopSpeaking()

Stops synthesis in progress.

macOS 10.3–14.0Deprecated

``` source
func stopSpeaking()
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Discussion

If the receiver is currently generating speech, synthesis is halted, and the message speechSynthesizer(_:didFinishSpeaking:) is sent to the delegate.

## See Also

### Synthesizing Speech

var isSpeaking: Bool

Indicates whether the receiver is currently generating synthesized speech.

Deprecated

func startSpeaking(String) -> Bool

Begins speaking synthesized text through the system’s default sound output device.

Deprecated

func startSpeaking(String, to: URL) -> Bool

Begins synthesizing text into a sound (AIFF) file.

Deprecated

func pauseSpeaking(at: NSSpeechSynthesizer.Boundary)

Pauses synthesis in progress at a given boundary.

Deprecated

func continueSpeaking()

Resumes synthesis.

Deprecated

func stopSpeaking(at: NSSpeechSynthesizer.Boundary)

Stops synthesis in progress at a given boundary.

Deprecated

enum Boundary

These constants are used to indicate where speech should be stopped and paused. See pauseSpeaking(at:) and stopSpeaking(at:).

Deprecated

