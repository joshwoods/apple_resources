

- Audio Toolbox
-  AudioQueueFreeBuffer(\_:\_:) 

Function

# AudioQueueFreeBuffer(\_:\_:)

Asks an audio queue to dispose of an audio queue buffer.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueFreeBuffer(
    _ inAQ: AudioQueueRef,
    _ inBuffer: AudioQueueBufferRef
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue that owns the audio queue buffer you want to dispose of.

`inBuffer`  

The buffer to dispose of.

## Return Value

A result code. See Result Codes.

## Discussion

Disposing of an audio queue also disposes of its buffers. Call this function only if you want to dispose of a particular buffer while continuing to use an audio queue. You can dispose of a buffer only when the audio queue that owns it is stopped (that is, not processing audio data).

## See Also

### Related Documentation

func AudioQueueDispose(AudioQueueRef, Bool) -> OSStatus

Disposes of an audio queue.

### Handling Audio Queue Buffers

func AudioQueueAllocateBuffer(AudioQueueRef, UInt32, UnsafeMutablePointer&lt;AudioQueueBufferRef?>) -> OSStatus

Asks an audio queue object to allocate an audio queue buffer.

func AudioQueueAllocateBufferWithPacketDescriptions(AudioQueueRef, UInt32, UInt32, UnsafeMutablePointer&lt;AudioQueueBufferRef?>) -> OSStatus

Asks an audio queue object to allocate an audio queue buffer with space for packet descriptions.

func AudioQueueEnqueueBuffer(AudioQueueRef, AudioQueueBufferRef, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?) -> OSStatus

Adds a buffer to the buffer queue of a recording or playback audio queue.

func AudioQueueEnqueueBufferWithParameters(AudioQueueRef, AudioQueueBufferRef, UInt32, UnsafePointer&lt;AudioStreamPacketDescription>?, UInt32, UInt32, UInt32, UnsafePointer&lt;AudioQueueParameterEvent>?, UnsafePointer&lt;AudioTimeStamp>?, UnsafeMutablePointer&lt;AudioTimeStamp>?) -> OSStatus

Adds a buffer to the buffer queue of a playback audio queue object, specifying start time and other settings.

