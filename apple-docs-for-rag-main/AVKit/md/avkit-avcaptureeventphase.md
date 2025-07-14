

- AVKit
-  AVCaptureEventPhase 

Enumeration

# AVCaptureEventPhase

Constants that indicate the phase of a system capture event.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+

``` source
enum AVCaptureEventPhase
```

## Topics

### Event phases

case began

A phase that indicates the beginning of a capture event.

case ended

A phase that indicates the end of a capture event.

case cancelled

A phase that indicates the cancellation of a capture event.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting the event

var phase: AVCaptureEventPhase

The current phase of a capture event.

