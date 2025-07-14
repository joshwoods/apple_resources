

- AVFAudio
-  AVAudioEngineManualRenderingError 

Enumeration

# AVAudioEngineManualRenderingError

Constants that describe error codes that the framework returns from manual rendering mode methods.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
enum AVAudioEngineManualRenderingError
```

## Topics

### Manual Rendering Errors

case initialized

An operation that the system can’t perform because the engine is still running.

case invalidMode

An operation the system can’t perform because the engine isn’t in manual rendering mode or the right variant of it.

case notRunning

An operation the system can’t perform because the engine isn’t running.

### Initializers

init?(rawValue: OSStatus)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum AVAudioEngineManualRenderingMode

The two modes for manual rendering.

enum AVAudioEngineManualRenderingStatus

Status codes that return from the render call to the engine operating in manual rendering mode.

