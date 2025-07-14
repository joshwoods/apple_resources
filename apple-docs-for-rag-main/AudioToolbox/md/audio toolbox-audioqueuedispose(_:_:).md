

- Audio Toolbox
-  AudioQueueDispose(\_:\_:) 

Function

# AudioQueueDispose(\_:\_:)

Disposes of an audio queue.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueDispose(
    _ inAQ: AudioQueueRef,
    _ inImmediate: Bool
) -> OSStatus
```

## Parameters 

`inAQ`  

The audio queue you want to dispose of.

`inImmediate`  

If you pass `true`, the audio queue is disposed of immediately (that is, synchronously). If you pass `false`, disposal does not take place until all enqueued buffers are processed (that is, asynchronously).

## Return Value

A result code. See Result Codes.

## Discussion

Disposing of an audio queue also disposes of its resources, including its buffers. After you call this function, you can no longer interact with the audio queue. In addition, the audio queue no longer invokes any callbacks.

## See Also

### Related Documentation

func AudioQueueFlush(AudioQueueRef) -> OSStatus

Resets an audio queue’s decoder state.

### Creating and Disposing of Audio Queues

func AudioQueueNewOutputWithDispatchQueue(UnsafeMutablePointer&lt;AudioQueueRef?>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, dispatch_queue_t, AudioQueueOutputCallbackBlock) -> OSStatus

func AudioQueueNewInputWithDispatchQueue(UnsafeMutablePointer&lt;AudioQueueRef?>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, dispatch_queue_t, AudioQueueInputCallbackBlock) -> OSStatus

func AudioQueueNewOutput(UnsafePointer&lt;AudioStreamBasicDescription>, AudioQueueOutputCallback, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, UInt32, UnsafeMutablePointer&lt;AudioQueueRef?>) -> OSStatus

Creates a new playback audio queue object.

func AudioQueueNewInput(UnsafePointer&lt;AudioStreamBasicDescription>, AudioQueueInputCallback, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, UInt32, UnsafeMutablePointer&lt;AudioQueueRef?>) -> OSStatus

Creates a new recording audio queue object.

typealias AudioQueueRef

Defines an opaque data type that represents an audio queue.

typealias AudioQueueInputCallbackBlock

typealias AudioQueueOutputCallbackBlock

