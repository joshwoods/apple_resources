

- AppKit
- NSSpeechSynthesizer
-  NSSpeechSynthesizer.Boundary Deprecated

Enumeration

# NSSpeechSynthesizer.Boundary

These constants are used to indicate where speech should be stopped and paused. See pauseSpeaking(at:) and stopSpeaking(at:).

macOS 10.5–14.0Deprecated

``` source
enum Boundary
```

Deprecated

Use AVSpeechSynthesizer in AVFoundation instead

## Topics

### Constants

case immediateBoundary

Speech should be paused or stopped immediately.

case wordBoundary

Speech should be paused or stopped at the end of the word.

case sentenceBoundary

Speech should be paused or stopped at the end of the sentence.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

func stopSpeaking()

Stops synthesis in progress.

Deprecated

func stopSpeaking(at: NSSpeechSynthesizer.Boundary)

Stops synthesis in progress at a given boundary.

Deprecated

