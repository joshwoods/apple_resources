

- AVFoundation
- AVSampleBufferRequest
-  AVSampleBufferRequest.Direction 

Enumeration

# AVSampleBufferRequest.Direction

The modes that describe the buffer request direction.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum Direction
```

## Topics

### Buffer Direction

case forward

The number of following samples may be zero or greater.

case none

A single sample will be loaded.

case reverse

The number of previous samples may be zero or greater.

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

var limitCursor: AVSampleCursor?

The limiting position for sample loading.

var maxSampleCount: Int

The maximum number of samples to load.

var mode: AVSampleBufferRequest.Mode

The sample buffer request mode.

enum Mode

The modes in which a sample buffer generator processes a request.

var overrideTime: CMTime

The deadline for sample data and output PTS for the sample buffer.

var preferredMinSampleCount: Int

The preferred minimum number of samples to load.

var startCursor: AVSampleCursor

The starting cursor position.

