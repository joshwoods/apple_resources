

- Core Audio Types
- AudioStreamPacketDescription
-  mVariableFramesInPacket 

Instance Property

# mVariableFramesInPacket

The number of sample frames of data in the packet.

iOS 2.0+iPadOS 2.0+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var mVariableFramesInPacket: UInt32
```

## Discussion

For formats with a constant number of frames per packet, this value is `0`.

## See Also

### Inspecting an audio stream packet description

var mDataByteSize: UInt32

The number of bytes in the packet.

var mStartOffset: Int64

The number of bytes from the start of the buffer to the beginning of the packet.

