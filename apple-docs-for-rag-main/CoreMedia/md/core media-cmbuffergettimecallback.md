

- Core Media
-  CMBufferGetTimeCallback 

Type Alias

# CMBufferGetTimeCallback

Callback that returns a `CMTime` from a `CMBuffer`.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMBufferGetTimeCallback = (CMBuffer, UnsafeMutableRawPointer?) -> CMTime
```

## Discussion

There are three callbacks of this type that can be provided to `Creating Buffer Queues`: getDuration (required), getDecodeTimeStamp (optional), and getPresentationTimeStamp (optional).

### Callback Parameters

buf  
The buffer being interrogated.

refcon  
The contextual data from the client (which may be `NULL`).

## See Also

### Properties

var compare: CMBufferCompareCallback?

This callback is called multiple times from CMBufferQueueEnqueue(_:buffer:), to perform an insertion sort.

typealias CMBufferCompareCallback

Callback that compares one `CMBuffer` with another.

typealias CMBufferGetBooleanCallback

Callback that returns a Boolean value from a `CMBuffer`.

var dataBecameReadyNotification: Unmanaged&lt;CFString>?

If triggers of type `kCMBufferQueueTrigger_WhenDataBecomesReady` are installed, the queue will listen for this notification on the head buffer.

var getDecodeTimeStamp: CMBufferGetTimeCallback?

Client callback that returns a `CMTime` from a `CMBuffer`.

var getDuration: CMBufferGetTimeCallback

This callback is called (once) during enqueue and dequeue operations to update the total duration of the queue.

var getPresentationTimeStamp: CMBufferGetTimeCallback?

Client callback that returns a `CMTime` from a `CMBuffer`.

var getSize: CMBufferGetSizeCallback?

var isDataReady: CMBufferGetBooleanCallback?

This callback is called from CMBufferQueueDequeueIfDataReady(_:), to ask if the buffer that is about to be dequeued is ready.

var refcon: UnsafeMutableRawPointer?

Contextual data to be passed to all callbacks.

var version: UInt32

The callback version.

