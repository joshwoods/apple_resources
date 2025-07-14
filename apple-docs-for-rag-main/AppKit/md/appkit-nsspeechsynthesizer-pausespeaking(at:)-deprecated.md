

- AppKit
- NSSpeechSynthesizer
-  pauseSpeaking(at:) Deprecated

Instance Method

# pauseSpeaking(at:)

Pauses synthesis in progress at a given boundary.

macOS 10.5–14.0Deprecated

``` source
func pauseSpeaking(at boundary: NSSpeechSynthesizer.Boundary)
```

## Parameters 

`boundary`  

Boundary at which to pause speech. The supported bound types are listed in NSSpeechSynthesizer.Boundary.

## Discussion

Pass the constant NSSpeechSynthesizer.Boundary.immediateBoundary to pause immediately, even in the middle of a word. Pass NSSpeechSynthesizer.Boundary.wordBoundary or NSSpeechSynthesizer.Boundary.sentenceBoundary to pause speech at the end of the current word or sentence, respectively.

You can determine whether your application has paused a synthesizer’s speech output by obtaining the status property through the object(forProperty:) method. While a synthesizer is paused, the speech status information indicates that outputBusy and outputPaused are both true.

If the end of the string being spoken is reached before the specified pause point, speech output pauses at the end of the string.

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

