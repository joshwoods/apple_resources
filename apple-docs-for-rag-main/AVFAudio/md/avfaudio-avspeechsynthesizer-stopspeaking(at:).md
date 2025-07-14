

- AVFAudio
- AVSpeechSynthesizer
-  stopSpeaking(at:) 

Instance Method

# stopSpeaking(at:)

Stops speech at the boundary you specify.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func stopSpeaking(at boundary: AVSpeechBoundary) -> Bool
```

## Parameters 

`boundary`  

An enumeration that describes whether to stop speech immediately or only after the synthesizer finishes speaking the current word.

## Return Value

true if speech stops; otherwise, false.

## Discussion

Unlike pausing a speech synthesizer, which can resume after a pause, stopping the synthesizer immediately cancels speech and removes all unspoken utterances from the synthesizer’s queue.

## See Also

### Controlling speech

func speak(AVSpeechUtterance)

Adds the utterance you specify to the speech synthesizer’s queue.

func continueSpeaking() -> Bool

Resumes speech from its paused point.

func pauseSpeaking(at: AVSpeechBoundary) -> Bool

Pauses speech at the boundary you specify.

enum AVSpeechBoundary

Specifies when to pause or stop speech.

