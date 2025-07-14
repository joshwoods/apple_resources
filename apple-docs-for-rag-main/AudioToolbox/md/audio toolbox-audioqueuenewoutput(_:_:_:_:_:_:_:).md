

- Audio Toolbox
-  AudioQueueNewOutput(\_:\_:\_:\_:\_:\_:\_:) 

Function

# AudioQueueNewOutput(\_:\_:\_:\_:\_:\_:\_:)

Creates a new playback audio queue object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+

``` source
func AudioQueueNewOutput(
    _ inFormat: UnsafePointer,
    _ inCallbackProc: AudioQueueOutputCallback,
    _ inUserData: UnsafeMutableRawPointer?,
    _ inCallbackRunLoop: CFRunLoop?,
    _ inCallbackRunLoopMode: CFString?,
    _ inFlags: UInt32,
    _ outAQ: UnsafeMutablePointer
) -> OSStatus
```

## Parameters 

`inFormat`  

The data format of the audio to play. For linear PCM, only interleaved formats are supported. Compressed formats are also supported.

`inCallbackProc`  

A callback function to use with the playback audio queue. The audio queue invokes the callback when the audio queue has finished acquiring a buffer. See AudioQueueOutputCallback.

`inUserData`  

A custom data structure for use with the callback function.

`inCallbackRunLoop`  

The event loop on which the callback function pointed to by the `inCallbackProc` parameter is to be called. If you specify `NULL`, the callback is invoked on one of the audio queue’s internal threads.

`inCallbackRunLoopMode`  

The run loop mode in which to invoke the callback function specified in the `inCallbackProc` parameter. Typically, you pass `kCFRunLoopCommonModes` or use `NULL`, which is equivalent. You can choose to create your own thread with your own run loops. For more information on run loops, see Run Loops and doc://com.apple.documentation/documentation/corefoundation/cfrunloop-rht.

`inFlags`  

Reserved for future use. Must be `0`.

`outAQ`  

On output, the newly created playback audio queue object.

## Return Value

A result code. See Result Codes.

## See Also

### Related Documentation

func AudioQueueOfflineRender(AudioQueueRef, UnsafePointer&lt;AudioTimeStamp>, AudioQueueBufferRef, UInt32) -> OSStatus

Exports audio to a buffer, instead of to a device, using a playback audio queue.

### Creating and Disposing of Audio Queues

func AudioQueueNewOutputWithDispatchQueue(UnsafeMutablePointer&lt;AudioQueueRef?>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, dispatch_queue_t, AudioQueueOutputCallbackBlock) -> OSStatus

func AudioQueueNewInputWithDispatchQueue(UnsafeMutablePointer&lt;AudioQueueRef?>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, dispatch_queue_t, AudioQueueInputCallbackBlock) -> OSStatus

func AudioQueueNewInput(UnsafePointer&lt;AudioStreamBasicDescription>, AudioQueueInputCallback, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, UInt32, UnsafeMutablePointer&lt;AudioQueueRef?>) -> OSStatus

Creates a new recording audio queue object.

func AudioQueueDispose(AudioQueueRef, Bool) -> OSStatus

Disposes of an audio queue.

typealias AudioQueueRef

Defines an opaque data type that represents an audio queue.

typealias AudioQueueInputCallbackBlock

typealias AudioQueueOutputCallbackBlock

