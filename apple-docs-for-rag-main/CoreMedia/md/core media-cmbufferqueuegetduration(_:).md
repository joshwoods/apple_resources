

- Core Media
-  CMBufferQueueGetDuration(\_:) 

Function

# CMBufferQueueGetDuration(\_:)

Gets the duration of a buffer queue.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueGetDuration(_ queue: CMBufferQueue) -> CMTime
```

## Parameters 

`queue`  

`CMBufferQueue` being interrogated.

## Return Value

Returns sum of all the individual buffer durations in the `CMBufferQueue`.

## Discussion

The duration of the `CMBufferQueue` is the sum of all the individual buffer durations, as reported by the `getDuration` callback (provided to `Creating Buffer Queues`). If there are no buffers in the queue, `kCMTimeZero` will be returned.

## See Also

### Inspecting Duration and Timing

func CMBufferQueueGetMinDecodeTimeStamp(CMBufferQueue) -> CMTime

Gets the earliest decode timestamp of a buffer queue.

func CMBufferQueueGetFirstDecodeTimeStamp(CMBufferQueue) -> CMTime

Gets the decode timestamp of the first buffer in a buffer queue.

func CMBufferQueueGetMinPresentationTimeStamp(CMBufferQueue) -> CMTime

Gets the earliest presentation timestamp of a buffer queue.

func CMBufferQueueGetFirstPresentationTimeStamp(CMBufferQueue) -> CMTime

Gets the presentation timestamp of the first buffer in a buffer queue.

func CMBufferQueueGetEndPresentationTimeStamp(CMBufferQueue) -> CMTime

Gets the greatest end presentation timestamp of a buffer queue.

func CMBufferQueueGetMaxPresentationTimeStamp(CMBufferQueue) -> CMTime

Gets the greatest presentation timestamp of a buffer queue.

func CMBufferQueueGetCallbacksForSampleBuffersSortedByOutputPTS() -> UnsafePointer&lt;CMBufferCallbacks>

Returns a pointer to a structure that contains callbacks to sort sample buffers by output presentation timestamp.

func CMBufferQueueGetCallbacksForUnsortedSampleBuffers() -> UnsafePointer&lt;CMBufferCallbacks>

Returns a pointer to a callback structure for unsorted sample buffers.

