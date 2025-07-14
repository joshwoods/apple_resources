

- Core Media
- CMBufferCallbacks
-  getPresentationTimeStamp 

Instance Property

# getPresentationTimeStamp

Client callback that returns a `CMTime` from a `CMBuffer`.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
var getPresentationTimeStamp: CMBufferGetTimeCallback?
```

## Discussion

This callback is called from once CMBufferQueueGetFirstPresentationTimeStamp(_:) and multiple times from CMBufferQueueGetMinPresentationTimeStamp(_:).

It should return the presentation timestamp of the buffer. If there are multiple samples in the buffer, this callback should return the minimum presentation timestamp in the buffer.

This can be `NULL` (CMBufferQueueGetFirstPresentationTimeStamp(_:) and CMBufferQueueGetMinPresentationTimeStamp(_:) will return `kCMTimeInvalid`).

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

var getDecodeTimeStamp: CMBufferGetTimeCallback?

Client callback that returns a `CMTime` from a `CMBuffer`.

var getDuration: CMBufferGetTimeCallback

This callback is called (once) during enqueue and dequeue operations to update the total duration of the queue.

var getSize: CMBufferGetSizeCallback?

var isDataReady: CMBufferGetBooleanCallback?

This callback is called from CMBufferQueueDequeueIfDataReady(_:), to ask if the buffer that is about to be dequeued is ready.

var refcon: UnsafeMutableRawPointer?

Contextual data to be passed to all callbacks.

var version: UInt32

The callback version.

