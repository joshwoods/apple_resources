

- Core Audio Types
-  AudioBufferList 

Structure

# AudioBufferList

A structure that stores a variable-length array of audio buffers.

iOS 2.0+iPadOS 2.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
struct AudioBufferList
```

## Topics

### Creating a Buffer List

init()

Creates an empty audio buffer list.

init(mNumberBuffers: UInt32, mBuffers: AudioBuffer)

Creates an audio buffer list with audio buffers.

### Accessing the Data

var mNumberBuffers: UInt32

The number of audio buffers in the list.

var mBuffers: AudioBuffer

A variable-length array of audio buffers.

### Type Methods

static func allocate(maximumBuffers: Int) -> UnsafeMutableAudioBufferListPointer

Allocate an `AudioBufferList` with a capacity for the specified number of `AudioBuffer`s.

static func sizeInBytes(maximumBuffers: Int) -> Int

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Buffers

struct AudioBuffer

A structure that holds a buffer of audio data.

