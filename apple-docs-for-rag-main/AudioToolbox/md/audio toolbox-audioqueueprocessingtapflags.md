

- Audio Toolbox
-  AudioQueueProcessingTapFlags 

Structure

# AudioQueueProcessingTapFlags

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioQueueProcessingTapFlags
```

## Topics

### Constants

static var endOfStream: AudioQueueProcessingTapFlags

static var postEffects: AudioQueueProcessingTapFlags

static var preEffects: AudioQueueProcessingTapFlags

static var siphon: AudioQueueProcessingTapFlags

static var startOfStream: AudioQueueProcessingTapFlags

### Initializers

init(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Data Types

struct AudioQueueChannelAssignment

struct AudioQueueBuffer

Defines an audio queue buffer.

typealias AudioQueueBufferRef

A pointer to an audio queue buffer.

struct AudioQueueLevelMeterState

Specifies the current level metering information for one channel of an audio queue.

struct AudioQueueParameterEvent

Specifies an audio queue parameter and associated value.

typealias AudioQueueParameterID

A `UInt32` value that uniquely identifies an audio queue parameter.

typealias AudioQueueParameterValue

A `Float32` value for an audio queue parameter.

typealias AudioQueueProcessingTapCallback

typealias AudioQueueProcessingTapRef

