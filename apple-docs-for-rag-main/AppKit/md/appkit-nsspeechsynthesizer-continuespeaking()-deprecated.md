

- AppKit
- NSSpeechSynthesizer
-  continueSpeaking() Deprecated

Instance Method

# continueSpeaking()

Resumes synthesis.

macOS 10.5–14.0Deprecated

``` source
func continueSpeaking()
```

## Discussion

At any time after pauseSpeaking(at:) is called, continueSpeaking() can be called to continue speaking from the beginning of the word at which speech paused.

Sending continueSpeaking() to a receiver that is not currently in a paused state has no effect on the synthesizer or on future calls to the pauseSpeaking(at:) function. If you call continueSpeaking() on a synthesizer before a pause is effective, continueSpeaking() cancels the pause.

If the pauseSpeaking(at:) method stopped speech in the middle of a word, the synthesizer will start speaking that word from the beginning when you call continueSpeaking().

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

func stopSpeaking()

Stops synthesis in progress.

Deprecated

func stopSpeaking(at: NSSpeechSynthesizer.Boundary)

Stops synthesis in progress at a given boundary.

Deprecated

enum Boundary

These constants are used to indicate where speech should be stopped and paused. See pauseSpeaking(at:) and stopSpeaking(at:).

Deprecated

