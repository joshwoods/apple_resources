

- Core Media
-  kCMBufferQueueError_BadTriggerDuration 

Global Variable

# kCMBufferQueueError_BadTriggerDuration

You specified an invalid trigger duration.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCMBufferQueueError_BadTriggerDuration: OSStatus { get }
```

## Discussion

The trigger duration must be numeric, and epoch must be zero (non-zero epoch is only for timestamps, not durations).

## See Also

### Error Codes

var kCMBufferQueueError_AllocationFailed: OSStatus

The system failed to allocate memory.

var kCMBufferQueueError_RequiredParameterMissing: OSStatus

You failed to provide a valid value for a required parameter.

var kCMBufferQueueError_InvalidCMBufferCallbacksStruct: OSStatus

The format of a callbacks structure isn’t correct.

var kCMBufferQueueError_EnqueueAfterEndOfData: OSStatus

You attempted to enqueue a buffer on a queue that disallows it.

var kCMBufferQueueError_QueueIsFull: OSStatus

You attempted to enqueue a buffer on a queue that’s full.

var kCMBufferQueueError_CannotModifyQueueFromTriggerCallback: OSStatus

A trigger callback attempted to modify a queue.

var kCMBufferQueueError_InvalidTriggerCondition: OSStatus

You specified an invalid trigger condition.

var kCMBufferQueueError_InvalidTriggerToken: OSStatus

You specified a trigger token that isn’t a trigger currently associated with this queue.

var kCMBufferQueueError_InvalidBuffer: OSStatus

A buffer validation callback rejected the buffer.

