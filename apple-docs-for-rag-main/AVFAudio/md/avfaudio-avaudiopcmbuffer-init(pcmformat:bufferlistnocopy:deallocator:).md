

- AVFAudio
- AVAudioPCMBuffer
-  init(pcmFormat:bufferListNoCopy:deallocator:) 

Initializer

# init(pcmFormat:bufferListNoCopy:deallocator:)

Creates a PCM audio buffer instance without copying samples, for PCM audio data, with a specified buffer list and a deallocator closure.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init?(
    pcmFormat format: AVAudioFormat,
    bufferListNoCopy bufferList: UnsafePointer,
    deallocator: ((UnsafePointer) -> Void)? = nil
)
```

## Parameters 

`format`  

The format of the PCM audio the buffer contains.

`bufferList`  

The buffer list with the memory to contain the PCM audio data.

`deallocator`  

The closure the method invokes when the resulting PCM buffer object deallocates.

## Return Value

A new AVAudioPCMBuffer instance, or `nil` if it’s not possible.

## Discussion

Use the deallocator parameter to define your own deallocation behavior for the audio buffer list’s underlying memory. The buffer list sent to the deallocator is identical to the one you specify, in term of buffer count and each buffer’s mData and mDataByteSize members.

The method returns `nil` due to the following reasons:

- The format has zero bytes per frame.

- The buffer you specify has zero number of buffers.

- The buffer list’s pointer to the buffer of audio data is in a `nil` state.

- Each of the buffer’s data byte size aren’t equal, or if any of the buffers’ data byte size is zero.

- There’s a mismatch between the format’s number of buffers and the buffer list’s size (1 if interleaved, mChannelsPerFrame if deinterleaved).

## See Also

### Creating a PCM Audio Buffer

init?(pcmFormat: AVAudioFormat, frameCapacity: AVAudioFrameCount)

Creates a PCM audio buffer instance for PCM audio data.

