

- Audio Toolbox
-  AudioQueueAllocateBuffer(\_:\_:\_:) 

Function

# AudioQueueAllocateBuffer(\_:\_:\_:)

Asks an audio queue object to allocate an audio queue buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueAllocateBuffer(
    _ inAQ: AudioQueueRef,
    _ inBufferByteSize: UInt32,
    _ outBuffer: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue you want to allocate a buffer.

`inBufferByteSize`  

The desired capacity of the new buffer, in bytes. Appropriate capacity depends on the processing you will perform on the data as well as on the audio data format.

`outBuffer`  

On output, points to the newly allocated audio queue buffer.

## Return Value

A result code. See Result Codes.

## Discussion

Once allocated, the pointer to the audio queue buffer and the buffer’s capacity cannot be changed. The buffer’s size field, `mAudioDataByteSize`, which indicates the amount of valid data, is initially set to 0.

## See Also

### Handling Audio Queue Buffers

func AudioQueueAllocateBufferWithPacketDescriptions(AudioQueueRef, UInt32, UInt32, UnsafeMutablePointer&lt;AudioQueueBufferRef?>) -> OSStatus

Asks an audio queue object to allocate an audio queue buffer with space for packet descriptions.

func AudioQueueFreeBuffer(AudioQueueRef, AudioQueueBufferRef) -> OSStatus

Asks an audio queue to dispose of an audio queue buffer.

func AudioQueueEnqueueBuffer(AudioQueueRef, AudioQueueBufferRef, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?) -> OSStatus

Adds a buffer to the buffer queue of a recording or playback audio queue.

func AudioQueueEnqueueBufferWithParameters(AudioQueueRef, AudioQueueBufferRef, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, UInt32, UInt32, UInt32, UnsafePointer&lt;AudioQueueParameterEvent>?, UnsafePointer&lt;AudioTimeStamp>?, UnsafeMutablePointer&lt;AudioTimeStamp>?) -> OSStatus

Adds a buffer to the buffer queue of a playback audio queue object, specifying start time and other settings.

