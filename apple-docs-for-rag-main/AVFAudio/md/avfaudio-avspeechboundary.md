

- AVFAudio
-  AVSpeechBoundary 

Enumeration

# AVSpeechBoundary

Specifies when to pause or stop speech.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.14+tvOSvisionOS 1.0+watchOS 2.0+

``` source
enum AVSpeechBoundary
```

## Topics

### Speech boundaries

case immediate

Indicates to pause or stop speech immediately.

case word

Indicates to pause or stop speech after the synthesizer finishes speaking the current word.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Controlling speech

func speak(AVSpeechUtterance)

Adds the utterance you specify to the speech synthesizer’s queue.

func continueSpeaking() -> Bool

Resumes speech from its paused point.

func pauseSpeaking(at: AVSpeechBoundary) -> Bool

Pauses speech at the boundary you specify.

func stopSpeaking(at: AVSpeechBoundary) -> Bool

Stops speech at the boundary you specify.

