

- Audio Toolbox
-  AudioQueueRef 

Type Alias

# AudioQueueRef

Defines an opaque data type that represents an audio queue.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias AudioQueueRef = OpaquePointer
```

## Discussion

An audio queue is a software object you use for recording or playing audio in macOS. It does the work of:

- Connecting to audio hardware

- Managing memory

- Employing codecs, as needed, for compressed audio formats

- Mediating recording or playback

You create, use, and dispose of audio queues using the functions described in Audio Queue Services.

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

typealias AudioQueueInputCallbackBlock

typealias AudioQueueOutputCallbackBlock

