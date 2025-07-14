

- AVFoundation
- AVSampleBufferRequest
-  AVSampleBufferRequest.Mode 

Enumeration

# AVSampleBufferRequest.Mode

The modes in which a sample buffer generator processes a request.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum Mode
```

## Topics

### Mode Scheduling

case immediate

A mode that indicates that sample buffer creation requests load data as soon as possible.

case scheduled

A mode that indicates that sample buffer creation requests load data according to a scheduled deadline.

case opportunistic

A mode that indicates that opportunistic sample buffer creation requests load data as soon as possible.

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

### Configuring Sample Buffer Request Parameters

var direction: AVSampleBufferRequest.Direction

The buffer sample direction.

enum Direction

The modes that describe the buffer request direction.

var limitCursor: AVSampleCursor?

The limiting position for sample loading.

var maxSampleCount: Int

The maximum number of samples to load.

var mode: AVSampleBufferRequest.Mode

The sample buffer request mode.

var overrideTime: CMTime

The deadline for sample data and output PTS for the sample buffer.

var preferredMinSampleCount: Int

The preferred minimum number of samples to load.

var startCursor: AVSampleCursor

The starting cursor position.

