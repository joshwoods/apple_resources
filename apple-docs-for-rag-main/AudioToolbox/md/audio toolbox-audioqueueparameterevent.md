

- Audio Toolbox
-  AudioQueueParameterEvent 

Structure

# AudioQueueParameterEvent

Specifies an audio queue parameter and associated value.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioQueueParameterEvent
```

## Overview

You use this structure with the AudioQueueEnqueueBufferWithParameters(_:_:_:_:_:_:_:_:_:_:) function. See that function, and Audio Queue Parameters, for more information.

## Topics

### Initializers

init()

init(mID: AudioQueueParameterID, mValue: AudioQueueParameterValue)

### Instance Properties

var mID: AudioQueueParameterID

The parameter.

var mValue: AudioQueueParameterValue

The value of the specified parameter.

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

struct AudioQueueLevelMeterState

Specifies the current level metering information for one channel of an audio queue.

typealias AudioQueueParameterID

A `UInt32` value that uniquely identifies an audio queue parameter.

typealias AudioQueueParameterValue

A `Float32` value for an audio queue parameter.

typealias AudioQueueProcessingTapCallback

typealias AudioQueueProcessingTapRef

