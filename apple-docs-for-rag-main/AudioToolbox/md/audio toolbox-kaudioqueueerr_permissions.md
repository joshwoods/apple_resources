

- Audio Toolbox
-  kAudioQueueErr_Permissions 

Global Variable

# kAudioQueueErr_Permissions

You do not have the required permissions to call the function.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
var kAudioQueueErr_Permissions: OSStatus { get }
```

## See Also

### Result Codes

var kAudioQueueErr_InvalidBuffer: OSStatus

The specified audio queue buffer does not belong to the specified audio queue.

var kAudioQueueErr_BufferEmpty: OSStatus

The audio queue buffer is empty (that is, the `mAudioDataByteSize` field = `0`).

var kAudioQueueErr_DisposalPending: OSStatus

The function cannot act on the audio queue because it is being asynchronously disposed of.

var kAudioQueueErr_InvalidProperty: OSStatus

The specified property ID is invalid.

var kAudioQueueErr_InvalidPropertySize: OSStatus

The size of the specified property is invalid.

var kAudioQueueErr_InvalidParameter: OSStatus

The specified parameter ID is invalid.

var kAudioQueueErr_CannotStart: OSStatus

The audio queue has encountered a problem and cannot start.

var kAudioQueueErr_InvalidDevice: OSStatus

The specified audio hardware device could not be located.

var kAudioQueueErr_BufferInQueue: OSStatus

The audio queue buffer cannot be disposed of when it is enqueued.

var kAudioQueueErr_InvalidRunState: OSStatus

The queue is running but the function can only operate on the queue when it is stopped, or vice versa.

var kAudioQueueErr_InvalidQueueType: OSStatus

The queue is an input queue but the function can only operate on an output queue, or vice versa.

var kAudioQueueErr_InvalidPropertyValue: OSStatus

The property value used is not valid.

var kAudioQueueErr_PrimeTimedOut: OSStatus

During a call to the AudioQueuePrime(_:_:_:) function, the audio queue’s audio converter failed to convert the requested number of sample frames.

var kAudioQueueErr_CodecNotFound: OSStatus

The requested codec was not found.

var kAudioQueueErr_InvalidCodecAccess: OSStatus

The codec could not be accessed.

