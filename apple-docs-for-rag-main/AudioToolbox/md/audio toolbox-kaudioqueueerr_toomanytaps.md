

- Audio Toolbox
-  kAudioQueueErr_TooManyTaps 

Global Variable

# kAudioQueueErr_TooManyTaps

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioQueueErr_TooManyTaps: OSStatus { get }
```

## See Also

### Constants

var kAudioQueueErr_BufferEmpty: OSStatus

The audio queue buffer is empty (that is, the `mAudioDataByteSize` field = `0`).

var kAudioQueueErr_BufferEnqueuedTwice: OSStatus

var kAudioQueueErr_BufferInQueue: OSStatus

The audio queue buffer cannot be disposed of when it is enqueued.

var kAudioQueueErr_CannotStart: OSStatus

The audio queue has encountered a problem and cannot start.

var kAudioQueueErr_CodecNotFound: OSStatus

The requested codec was not found.

var kAudioQueueErr_DisposalPending: OSStatus

The function cannot act on the audio queue because it is being asynchronously disposed of.

var kAudioQueueErr_EnqueueDuringReset: OSStatus

During a call to the AudioQueueReset(_:), AudioQueueStop(_:_:), or AudioQueueDispose(_:_:) functions, the system does not allow you to enqueue buffers.

var kAudioQueueErr_InvalidBuffer: OSStatus

The specified audio queue buffer does not belong to the specified audio queue.

var kAudioQueueErr_InvalidCodecAccess: OSStatus

The codec could not be accessed.

var kAudioQueueErr_InvalidDevice: OSStatus

The specified audio hardware device could not be located.

var kAudioQueueErr_InvalidOfflineMode: OSStatus

The operation requires the audio queue to be in offline mode but it isn’t, or vice versa.

var kAudioQueueErr_InvalidParameter: OSStatus

The specified parameter ID is invalid.

var kAudioQueueErr_InvalidProperty: OSStatus

The specified property ID is invalid.

var kAudioQueueErr_InvalidPropertySize: OSStatus

The size of the specified property is invalid.

var kAudioQueueErr_InvalidPropertyValue: OSStatus

The property value used is not valid.

