

- AVFAudio
- AVSpeechSynthesizer
-  continueSpeaking() 

Instance Method

# continueSpeaking()

Resumes speech from its paused point.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func continueSpeaking() -> Bool
```

## Return Value

true if speech resumes; otherwise, false.

## Discussion

This method only has an effect if the speech synthesizer is in a paused state.

## See Also

### Controlling speech

func speak(AVSpeechUtterance)

Adds the utterance you specify to the speech synthesizer’s queue.

func pauseSpeaking(at: AVSpeechBoundary) -> Bool

Pauses speech at the boundary you specify.

func stopSpeaking(at: AVSpeechBoundary) -> Bool

Stops speech at the boundary you specify.

enum AVSpeechBoundary

Specifies when to pause or stop speech.

