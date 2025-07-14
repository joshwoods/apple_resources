

- Core Media
- CMBufferCallbacks
-  getDecodeTimeStamp 

Instance Property

# getDecodeTimeStamp

Client callback that returns a `CMTime` from a `CMBuffer`.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
var getDecodeTimeStamp: CMBufferGetTimeCallback?
```

## Discussion

This callback is called once from CMBufferQueueGetFirstDecodeTimeStamp(_:) and multiple times from CMBufferQueueGetMinDecodeTimeStamp(_:).

It should return the decode timestamp of the buffer. If there are multiple samples in the buffer, this callback should return the minimum decode timestamp in the buffer.

This can be `NULL` (CMBufferQueueGetFirstDecodeTimeStamp(_:) and CMBufferQueueGetMinDecodeTimeStamp(_:) will return `kCMTimeInvalid`).

## See Also

### Properties

var compare: CMBufferCompareCallback?

This callback is called multiple times from CMBufferQueueEnqueue(_:buffer:), to perform an insertion sort.

typealias CMBufferCompareCallback

Callback that compares one `CMBuffer` with another.

typealias CMBufferGetBooleanCallback

Callback that returns a Boolean value from a `CMBuffer`.

typealias CMBufferGetTimeCallback

Callback that returns a `CMTime` from a `CMBuffer`.

var dataBecameReadyNotification: Unmanaged&lt;CFString>?

If triggers of type `kCMBufferQueueTrigger_WhenDataBecomesReady` are installed, the queue will listen for this notification on the head buffer.

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

