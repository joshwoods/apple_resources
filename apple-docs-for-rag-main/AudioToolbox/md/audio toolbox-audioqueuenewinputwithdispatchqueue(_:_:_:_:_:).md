

- Audio Toolbox
-  AudioQueueNewInputWithDispatchQueue(\_:\_:\_:\_:\_:) 

Function

# AudioQueueNewInputWithDispatchQueue(\_:\_:\_:\_:\_:)

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.6+tvOS 10.0+visionOS 1.0+

``` source
func AudioQueueNewInputWithDispatchQueue(
    _ outAQ: UnsafeMutablePointer,
    _ inFormat: UnsafePointer,
    _ inFlags: UInt32,
    _ inCallbackDispatchQueue: dispatch_queue_t,
    _ inCallbackBlock: @escaping AudioQueueInputCallbackBlock
) -> OSStatus
```

## See Also

### Creating and Disposing of Audio Queues

func AudioQueueNewOutputWithDispatchQueue(UnsafeMutablePointer&lt;AudioQueueRef?>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, dispatch_queue_t, AudioQueueOutputCallbackBlock) -> OSStatus

func AudioQueueNewOutput(UnsafePointer&lt;AudioStreamBasicDescription>, AudioQueueOutputCallback, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, UInt32, UnsafeMutablePointer&lt;AudioQueueRef?>) -> OSStatus

Creates a new playback audio queue object.

func AudioQueueNewInput(UnsafePointer&lt;AudioStreamBasicDescription>, AudioQueueInputCallback, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, UInt32, UnsafeMutablePointer&lt;AudioQueueRef?>) -> OSStatus

Creates a new recording audio queue object.

func AudioQueueDispose(AudioQueueRef, Bool) -> OSStatus

Disposes of an audio queue.

typealias AudioQueueRef

Defines an opaque data type that represents an audio queue.

typealias AudioQueueInputCallbackBlock

typealias AudioQueueOutputCallbackBlock

