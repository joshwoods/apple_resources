

- AVFoundation
- AVCaptureOutput
-  AVCaptureOutput.DataDroppedReason 

Enumeration

# AVCaptureOutput.DataDroppedReason

Constants that define reasons for why the system dropped a frame.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+macOS 10.15+tvOS 17.0+visionOS 1.0+

``` source
enum DataDroppedReason
```

## Topics

### Reasons

case none

The system didn’t drop data.

case lateData

The system dropped data because you’ve configured capture output to drop data when delegate queue is in a blocked state, and there’s data to deliver.

case outOfBuffers

The system dropped data because the capture output exhausted its internal pool of memory buffers.

case discontinuity

The system dropped data because the device providing data experienced a discontinuity, and the output lost an unknown number of data objects.

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

### Accessing Connections

var connections: [AVCaptureConnection]

The capture output object’s connections.

func connection(with: AVMediaType) -> AVCaptureConnection?

Returns the first connection with an input port of a specified media type.

