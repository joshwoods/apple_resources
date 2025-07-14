

- AVFAudio
- AVSpeechSynthesizer
-  speak(\_:) 

Instance Method

# speak(\_:)

Adds the utterance you specify to the speech synthesizer’s queue.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func speak(_ utterance: AVSpeechUtterance)
```

## Parameters 

`utterance`  

An AVSpeechUtterance instance that contains text to speak.

## Discussion

Warning

Attempting to enqueue the same utterance more than once throws an exception.

## See Also

### Controlling speech

func continueSpeaking() -> Bool

Resumes speech from its paused point.

func pauseSpeaking(at: AVSpeechBoundary) -> Bool

Pauses speech at the boundary you specify.

func stopSpeaking(at: AVSpeechBoundary) -> Bool

Stops speech at the boundary you specify.

enum AVSpeechBoundary

Specifies when to pause or stop speech.

