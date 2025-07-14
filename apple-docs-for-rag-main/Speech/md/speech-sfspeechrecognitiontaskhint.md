

- Speech
-  SFSpeechRecognitionTaskHint 

Enumeration

# SFSpeechRecognitionTaskHint

The type of task for which you are using speech recognition.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
enum SFSpeechRecognitionTaskHint
```

## Topics

### Hints

case unspecified

An unspecified type of task.

case dictation

A task that uses captured speech for text entry.

case search

A task that uses captured speech to specify search terms.

case confirmation

A task that uses captured speech for short, confirmation-style requests.

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

### Speech Type Classification

var taskHint: SFSpeechRecognitionTaskHint

A value that indicates the type of speech recognition being performed.

