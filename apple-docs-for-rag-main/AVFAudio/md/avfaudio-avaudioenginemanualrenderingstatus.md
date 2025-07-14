

- AVFAudio
-  AVAudioEngineManualRenderingStatus 

Enumeration

# AVAudioEngineManualRenderingStatus

Status codes that return from the render call to the engine operating in manual rendering mode.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum AVAudioEngineManualRenderingStatus
```

## Topics

### Constants

case error

A problem that occurs during rendering and results in no data returning.

case success

A status that indicates the successful return of the requested data.

case insufficientDataFromInputNode

A condition that occurs when the input node doesn’t return enough input data to satisfy the render request at the time of the request.

case cannotDoInCurrentContext

An operation that the system can’t perform under the current conditions.

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

### Constants

enum AVAudioEngineManualRenderingError

Constants that describe error codes that the framework returns from manual rendering mode methods.

enum AVAudioEngineManualRenderingMode

The two modes for manual rendering.

