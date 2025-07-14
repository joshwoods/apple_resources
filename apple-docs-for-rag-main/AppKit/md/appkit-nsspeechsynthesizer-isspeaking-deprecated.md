

- AppKit
- NSSpeechSynthesizer
-  isSpeaking Deprecated

Instance Property

# isSpeaking

Indicates whether the receiver is currently generating synthesized speech.

macOS 10.3–14.0Deprecated

``` source
var isSpeaking: Bool { get }
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Discussion

true when the receiver is generating synthesized speech, false otherwise.

## See Also

### Synthesizing Speech

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

func stopSpeaking()

Stops synthesis in progress.

Deprecated

func stopSpeaking(at: NSSpeechSynthesizer.Boundary)

Stops synthesis in progress at a given boundary.

Deprecated

enum Boundary

These constants are used to indicate where speech should be stopped and paused. See pauseSpeaking(at:) and stopSpeaking(at:).

Deprecated

