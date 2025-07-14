

- Core Audio Types
- AudioStreamPacketDescription
-  init(mStartOffset:mVariableFramesInPacket:mDataByteSize:) 

Initializer

# init(mStartOffset:mVariableFramesInPacket:mDataByteSize:)

Creates an audio stream basic description with the start offset, and the number of sample frames and bytes in the packet that you specify.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    mStartOffset: Int64,
    mVariableFramesInPacket: UInt32,
    mDataByteSize: UInt32
)
```

## Parameters 

`mStartOffset`  

The number of bytes from the start of the buffer to the beginning of the packet.

`mVariableFramesInPacket`  

The number of sample frames of data in the packet. For formats with a constant number of frames per packet, set this to `0`.

`mDataByteSize`  

The number of bytes in the packet.

## See Also

### Creating an audio stream packet descripiton

init()

Creates an audio stream basic description.

