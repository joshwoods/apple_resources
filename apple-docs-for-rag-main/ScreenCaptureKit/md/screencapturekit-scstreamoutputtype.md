

- ScreenCaptureKit
-  SCStreamOutputType 

Enumeration

# SCStreamOutputType

Constants that represent output types for a stream frame.

Mac Catalyst 18.2+macOS 12.3+

``` source
enum SCStreamOutputType
```

## Topics

### Output types

case screen

An output type that represents a screen capture sample buffer.

case audio

An output type that represents an audio capture sample buffer.

### Enumeration Cases

case microphone

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

### Output processing

protocol SCStreamOutput

A delegate protocol your app implements to receive capture stream output events.

struct SCStreamFrameInfo

An instance that defines metadata keys for a stream frame.

enum SCFrameStatus

Status values for a frame from a stream.

