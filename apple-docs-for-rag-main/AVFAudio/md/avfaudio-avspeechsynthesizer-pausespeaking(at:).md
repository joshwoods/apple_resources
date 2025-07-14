

- AVFAudio
- AVSpeechSynthesizer
-  pauseSpeaking(at:) 

Instance Method

# pauseSpeaking(at:)

Pauses speech at the boundary you specify.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func pauseSpeaking(at boundary: AVSpeechBoundary) -> Bool
```

## Parameters 

`boundary`  

An enumeration that describes whether to pause speech immediately or only after the synthesizer finishes speaking the current word.

## Return Value

true if speech pauses; otherwise, false.

## Discussion

The `boundary` parameter also affects how the speech synthesizer resumes speaking text after a pause and call to continueSpeaking(). If the boundary is AVSpeechBoundary.immediate, speech resumes from the exact point where it pauses, even if that point occurs in the middle of speaking a word. If the boundary is AVSpeechBoundary.word, speech resumes from the word that follows the last spoken word where it pauses.

## See Also

### Controlling speech

func speak(AVSpeechUtterance)

Adds the utterance you specify to the speech synthesizer’s queue.

func continueSpeaking() -> Bool

Resumes speech from its paused point.

func stopSpeaking(at: AVSpeechBoundary) -> Bool

Stops speech at the boundary you specify.

enum AVSpeechBoundary

Specifies when to pause or stop speech.

