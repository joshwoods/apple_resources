

- Core Media
-  CMBufferCallbacks 

Structure

# CMBufferCallbacks

A structure that stores the callbacks that perform buffer operations.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
struct CMBufferCallbacks
```

## Overview

With the exception of `isDataReady`, all these callbacks must always return the same result for the same arguments.

A buffer’s duration, timestamps, or position relative to other buffers must not appear to change while it is in the queue. Once `isDataReady` has returned true for a given `CMBuffer`, it must always return true for that `CMBuffer`.

Durations must always be positive.

## Topics

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

var getPresentationTimeStamp: CMBufferGetTimeCallback?

Client callback that returns a `CMTime` from a `CMBuffer`.

var getSize: CMBufferGetSizeCallback?

var isDataReady: CMBufferGetBooleanCallback?

This callback is called from CMBufferQueueDequeueIfDataReady(_:), to ask if the buffer that is about to be dequeued is ready.

var refcon: UnsafeMutableRawPointer?

Contextual data to be passed to all callbacks.

var version: UInt32

The callback version.

### Initializers

init(version: UInt32, refcon: UnsafeMutableRawPointer?, getDecodeTimeStamp: CMBufferGetTimeCallback?, getPresentationTimeStamp: CMBufferGetTimeCallback?, getDuration: CMBufferGetTimeCallback, isDataReady: CMBufferGetBooleanCallback?, compare: CMBufferCompareCallback?, dataBecameReadyNotification: Unmanaged&lt;CFString>?, getSize: CMBufferGetSizeCallback?)

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Creating a Queue

func CMBufferQueueCreateWithHandlers(CFAllocator?, CMItemCount, OpaquePointer, UnsafeMutablePointer&lt;CMBufferQueue?>) -> OSStatus

Creates a buffer queue with handlers to inspect buffers.

func CMBufferQueueCreate(allocator: CFAllocator?, capacity: CMItemCount, callbacks: UnsafePointer&lt;CMBufferCallbacks>, queueOut: UnsafeMutablePointer&lt;CMBufferQueue?>) -> OSStatus

Creates a buffer queue with callbacks to inspect buffers.

