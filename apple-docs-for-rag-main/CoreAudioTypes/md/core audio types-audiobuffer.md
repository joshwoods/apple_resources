

- Core Audio Types
-  AudioBuffer 

Structure

# AudioBuffer

A structure that holds a buffer of audio data.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct AudioBuffer
```

## Overview

An audio buffer holds a single buffer of audio data in its mData field. The buffer can represent two types of audio:

- A single, monophonic, noninterleaved channel of audio

- Interleaved audio with the number of channels set by the mNumberChannels field

Note

The mDataByteSize and mNumberChannels parameters needs to match the memory layout of mData, so update the size and number of channels when you update the data field.

## Topics

### Creating a Buffer

init()

Creates an empty audio buffer.

init(mNumberChannels: UInt32, mDataByteSize: UInt32, mData: UnsafeMutableRawPointer?)

Creates an audio buffer with audio data.

### Accessing the Audio

var mNumberChannels: UInt32

The number of interleaved channels in the buffer.

var mDataByteSize: UInt32

The number of bytes in the buffer.

var mData: UnsafeMutableRawPointer?

A pointer to a buffer of audio data.

### Initializers

init&lt;Element>(UnsafeMutableBufferPointer&lt;Element>, numberOfChannels: Int)

Initialize an `AudioBuffer` from an `UnsafeMutableBufferPointer`.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Buffers

struct AudioBufferList

A structure that stores a variable-length array of audio buffers.

