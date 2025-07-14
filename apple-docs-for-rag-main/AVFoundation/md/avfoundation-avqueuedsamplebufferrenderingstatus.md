

- AVFoundation
-  AVQueuedSampleBufferRenderingStatus 

Enumeration

# AVQueuedSampleBufferRenderingStatus

The statuses for sample buffer rendering.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.2+visionOS 1.0+watchOS 1.0+

``` source
enum AVQueuedSampleBufferRenderingStatus
```

## Topics

### Status Values

case unknown

The object doesn’t have any sample buffers enqueued.

case rendering

The object is rendering the sample buffer.

case failed

The object can no longer render sample buffers because of an error.

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

### Determining Rendering Status

var status: AVQueuedSampleBufferRenderingStatus

The status of the audio renderer.

