

- AppKit
- NSSpeechSynthesizer
-  stopSpeaking(at:) Deprecated

Instance Method

# stopSpeaking(at:)

Stops synthesis in progress at a given boundary.

macOS 10.5–14.0Deprecated

``` source
func stopSpeaking(at boundary: NSSpeechSynthesizer.Boundary)
```

## Parameters 

`boundary`  

Boundary at which to stop speech. The supported bound types are listed in NSSpeechSynthesizer.Boundary.

## Discussion

Pass the constant NSSpeechSynthesizer.Boundary.immediateBoundary to stop immediately, even in the middle of a word. Pass NSSpeechSynthesizer.Boundary.wordBoundary or NSSpeechSynthesizer.Boundary.sentenceBoundary to stop speech at the end of the current word or sentence, respectively.

If the end of the string being spoken is reached before the specified stopping point, the synthesizer stops at the end of the string without generating an error.

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

enum Boundary

These constants are used to indicate where speech should be stopped and paused. See pauseSpeaking(at:) and stopSpeaking(at:).

Deprecated

