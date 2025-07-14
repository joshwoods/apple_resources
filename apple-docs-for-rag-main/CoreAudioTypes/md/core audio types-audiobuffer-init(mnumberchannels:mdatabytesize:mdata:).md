

- Core Audio Types
- AudioBuffer
-  init(mNumberChannels:mDataByteSize:mData:) 

Initializer

# init(mNumberChannels:mDataByteSize:mData:)

Creates an audio buffer with audio data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    mNumberChannels: UInt32,
    mDataByteSize: UInt32,
    mData: UnsafeMutableRawPointer?
)
```

## Parameters 

`mNumberChannels`  

The number of interleaved channels in the buffer.

`mDataByteSize`  

The number of bytes in the buffer.

`mData`  

A pointer to a buffer of audio data.

## See Also

### Creating a Buffer

init()

Creates an empty audio buffer.

