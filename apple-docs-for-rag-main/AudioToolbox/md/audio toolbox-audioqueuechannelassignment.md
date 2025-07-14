

- Audio Toolbox
-  AudioQueueChannelAssignment 

Structure

# AudioQueueChannelAssignment

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioQueueChannelAssignment
```

## Topics

### Initializers

init(mDeviceUID: Unmanaged&lt;CFString>, mChannelNumber: UInt32)

### Instance Properties

var mChannelNumber: UInt32

var mDeviceUID: Unmanaged&lt;CFString>

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct AudioQueueProcessingTapFlags

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

