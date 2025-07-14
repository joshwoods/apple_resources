

- Audio Toolbox
-  AudioQueueNewInput(\_:\_:\_:\_:\_:\_:\_:) 

Function

# AudioQueueNewInput(\_:\_:\_:\_:\_:\_:\_:)

Creates a new recording audio queue object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueNewInput(
    _ inFormat: UnsafePointer,
    _ inCallbackProc: AudioQueueInputCallback,
    _ inUserData: UnsafeMutableRawPointer?,
    _ inCallbackRunLoop: CFRunLoop?,
    _ inCallbackRunLoopMode: CFString?,
    _ inFlags: UInt32,
    _ outAQ: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inFormat`  

The compressed or uncompressed audio data format to record to. When recording to linear PCM, only interleaved formats are supported.

`inCallbackProc`  

A callback function to use with the recording audio queue. The audio queue calls this function when the audio queue has finished filling a buffer. See AudioQueueInputCallback.

`inUserData`  

A custom data structure for use with the callback function.

`inCallbackRunLoop`  

The event loop on which the callback function pointed to by the `inCallbackProc` parameter is to be called. If you specify `NULL`, the callback is called on one of the audio queue’s internal threads.

`inCallbackRunLoopMode`  

The run loop mode in which to invoke the callback function specified in the `inCallbackProc` parameter. Typically, you pass `kCFRunLoopCommonModes` or use `NULL`, which is equivalent. You can choose to create your own thread with your own run loops. For more information on run loops, see Run Loops and doc://com.apple.documentation/documentation/corefoundation/cfrunloop-rht.

`inFlags`  

Reserved for future use. Must be `0`.

`outAQ`  

On output, the newly created recording audio queue.

## Return Value

A result code. See Result Codes.

## See Also

### Related Documentation

func AudioQueueSetOfflineRenderFormat(AudioQueueRef, UnsafePointer&lt;AudioStreamBasicDescription>?, UnsafePointer&lt;AudioChannelLayout>?) -> OSStatus

Sets the rendering mode and audio format for a playback audio queue.

### Creating and Disposing of Audio Queues

func AudioQueueNewOutputWithDispatchQueue(UnsafeMutablePointer&lt;AudioQueueRef?>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, dispatch_queue_t, AudioQueueOutputCallbackBlock) -> OSStatus

func AudioQueueNewInputWithDispatchQueue(UnsafeMutablePointer&lt;AudioQueueRef?>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, dispatch_queue_t, AudioQueueInputCallbackBlock) -> OSStatus

func AudioQueueNewOutput(UnsafePointer&lt;AudioStreamBasicDescription>, AudioQueueOutputCallback, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, UInt32, UnsafeMutablePointer&lt;AudioQueueRef?>) -> OSStatus

Creates a new playback audio queue object.

func AudioQueueDispose(AudioQueueRef, Bool) -> OSStatus

Disposes of an audio queue.

typealias AudioQueueRef

Defines an opaque data type that represents an audio queue.

typealias AudioQueueInputCallbackBlock

typealias AudioQueueOutputCallbackBlock

