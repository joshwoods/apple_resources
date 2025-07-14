

- Core Audio Types
- AudioStreamBasicDescription
-  init(mSampleRate:mFormatID:mFormatFlags:mBytesPerPacket:mFramesPerPacket:mBytesPerFrame:mChannelsPerFrame:mBitsPerChannel:mReserved:) 

Initializer

# init(mSampleRate:mFormatID:mFormatFlags:mBytesPerPacket:mFramesPerPacket:mBytesPerFrame:mChannelsPerFrame:mBitsPerChannel:mReserved:)

Creates a description with the specified values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    mSampleRate: Float64,
    mFormatID: AudioFormatID,
    mFormatFlags: AudioFormatFlags,
    mBytesPerPacket: UInt32,
    mFramesPerPacket: UInt32,
    mBytesPerFrame: UInt32,
    mChannelsPerFrame: UInt32,
    mBitsPerChannel: UInt32,
    mReserved: UInt32
)
```

## See Also

### Initializers

init()

Creates an empty description.

