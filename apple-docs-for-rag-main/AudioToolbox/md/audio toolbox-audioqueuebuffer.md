

- Audio Toolbox
-  AudioQueueBuffer 

Structure

# AudioQueueBuffer

Defines an audio queue buffer.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct AudioQueueBuffer
```

## Overview

Each audio queue has an associated set of audio queue buffers. To allocate a buffer, call the AudioQueueAllocateBuffer(_:_:_:) function. To dispose of a buffer, call the AudioQueueFreeBuffer(_:_:) function.

If using a VBR compressed audio data format, you may want to instead use the `AudioQueueAllocateBufferWithPacketDescriptions` function. This function allocates a buffer with additional space for packet descriptions. The `mPacketDescriptionCapacity`, `mPacketDescriptions`, and `mPacketDescriptionCount` fields may only be used with buffers allocated with `AudioQueueAllocateBufferWithPacketDescriptions`.

## Topics

### Initializers

init(mAudioDataBytesCapacity: UInt32, mAudioData: UnsafeMutableRawPointer, mAudioDataByteSize: UInt32, mUserData: UnsafeMutableRawPointer?, mPacketDescriptionCapacity: UInt32, mPacketDescriptions: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?, mPacketDescriptionCount: UInt32)

### Instance Properties

var mAudioData: UnsafeMutableRawPointer

The audio data owned the audio queue buffer. The buffer address cannot be changed.

var mAudioDataByteSize: UInt32

The number of bytes of valid audio data in the audio queue buffer’s `mAudioData` field, initially set to `0`. Your callback must set this value for a playback audio queue; for recording, the recording audio queue sets the value.

var mAudioDataBytesCapacity: UInt32

The size of the audio queue buffer, in bytes. This size is set when a buffer is allocated and cannot be changed.

var mPacketDescriptionCapacity: UInt32

The maximum number of packet descriptions that can be stored in the `mPacketDescriptions` field.

var mPacketDescriptionCount: UInt32

The number of valid packet descriptions in the buffer. You set this value when providing buffers for playback. The audio queue sets this value when returning buffers from a recording queue.

var mPacketDescriptions: UnsafeMutablePointer&lt;AudioStreamPacketDescription>?

An array of `AudioStreamPacketDescription` structures for the buffer.

var mUserData: UnsafeMutableRawPointer?

The custom data structure you specify, for use by your callback function, when creating a recording or playback audio queue.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

struct AudioQueueChannelAssignment

struct AudioQueueProcessingTapFlags

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

