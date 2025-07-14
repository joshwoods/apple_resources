

- Core Audio Types
- AudioBufferList
-  init(mNumberBuffers:mBuffers:) 

Initializer

# init(mNumberBuffers:mBuffers:)

Creates an audio buffer list with audio buffers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    mNumberBuffers: UInt32,
    mBuffers: AudioBuffer
)
```

## Parameters 

`mNumberBuffers`  

The number of audio buffers in the list.

`mBuffers`  

A variable-length array of audio buffers.

## See Also

### Creating a Buffer List

init()

Creates an empty audio buffer list.

