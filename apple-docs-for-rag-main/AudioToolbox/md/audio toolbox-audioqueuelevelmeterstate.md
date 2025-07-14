

- Audio Toolbox
-  AudioQueueLevelMeterState 

Structure

# AudioQueueLevelMeterState

Specifies the current level metering information for one channel of an audio queue.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioQueueLevelMeterState
```

## Topics

### Initializers

init()

init(mAveragePower: Float32, mPeakPower: Float32)

### Instance Properties

var mAveragePower: Float32

The audio channel’s average RMS power.

var mPeakPower: Float32

The audio channel’s peak RMS power.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct AudioQueueChannelAssignment

struct AudioQueueProcessingTapFlags

struct AudioQueueBuffer

Defines an audio queue buffer.

typealias AudioQueueBufferRef

A pointer to an audio queue buffer.

struct AudioQueueParameterEvent

Specifies an audio queue parameter and associated value.

typealias AudioQueueParameterID

A `UInt32` value that uniquely identifies an audio queue parameter.

typealias AudioQueueParameterValue

A `Float32` value for an audio queue parameter.

typealias AudioQueueProcessingTapCallback

typealias AudioQueueProcessingTapRef

