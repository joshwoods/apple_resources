

- Core Media
-  CMBufferCompareCallback 

Type Alias

# CMBufferCompareCallback

Callback that compares one `CMBuffer` with another.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
typealias CMBufferCompareCallback = (CMBuffer, CMBuffer, UnsafeMutableRawPointer?) -> CFComparisonResult
```

## Discussion

You can use a `CFComparatorFunction` as a callback.

### Callback parameters

buf1  
The first buffer being compared.

buf2  
The second buffer being compared.

refcon  
The contextual data from the client (which may be `NULL`).

## See Also

### Properties

var compare: CMBufferCompareCallback?

This callback is called multiple times from CMBufferQueueEnqueue(_:buffer:), to perform an insertion sort.

typealias CMBufferGetBooleanCallback

Callback that returns a Boolean value from a `CMBuffer`.

typealias CMBufferGetTimeCallback

Callback that returns a `CMTime` from a `CMBuffer`.

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

