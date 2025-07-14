

- Speech
-  SFSpeechRecognitionTaskState 

Enumeration

# SFSpeechRecognitionTaskState

The state of the task associated with the recognition request.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
enum SFSpeechRecognitionTaskState
```

## Topics

### Constants

case canceling

Delivery of recognition results has finished, but audio recording may be ongoing.

case completed

Delivery of recognition requests has finished and audio recording has stopped.

case finishing

Audio recording has stopped, but delivery of recognition results may continue.

case running

Speech recognition (potentially including audio recording) is in progress.

case starting

Speech recognition (potentially including audio recording) has not yet started.

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

### Monitoring Recognition Progress

var state: SFSpeechRecognitionTaskState

The current state of the speech recognition task.

var error: (any Error)?

An error object that specifies the error that occurred during a speech recognition task.

