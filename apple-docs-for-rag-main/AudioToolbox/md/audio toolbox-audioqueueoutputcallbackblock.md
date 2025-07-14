

- Audio Toolbox
-  AudioQueueOutputCallbackBlock 

Type Alias

# AudioQueueOutputCallbackBlock

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioQueueOutputCallbackBlock = (AudioQueueRef, AudioQueueBufferRef) -> Void
```

## See Also

### Creating and Disposing of Audio Queues

func AudioQueueNewOutputWithDispatchQueue(UnsafeMutablePointer&lt;AudioQueueRef?>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, dispatch_queue_t, AudioQueueOutputCallbackBlock) -> OSStatus

func AudioQueueNewInputWithDispatchQueue(UnsafeMutablePointer&lt;AudioQueueRef?>, UnsafePointer&lt;AudioStreamBasicDescription>, UInt32, dispatch_queue_t, AudioQueueInputCallbackBlock) -> OSStatus

func AudioQueueNewOutput(UnsafePointer&lt;AudioStreamBasicDescription>, AudioQueueOutputCallback, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, UInt32, UnsafeMutablePointer&lt;AudioQueueRef?>) -> OSStatus

Creates a new playback audio queue object.

func AudioQueueNewInput(UnsafePointer&lt;AudioStreamBasicDescription>, AudioQueueInputCallback, UnsafeMutableRawPointer?, CFRunLoop?, CFString?, UInt32, UnsafeMutablePointer&lt;AudioQueueRef?>) -> OSStatus

Creates a new recording audio queue object.

func AudioQueueDispose(AudioQueueRef, Bool) -> OSStatus

Disposes of an audio queue.

typealias AudioQueueRef

Defines an opaque data type that represents an audio queue.

typealias AudioQueueInputCallbackBlock

