

- Core Media
-  CMBufferQueueGetCallbacksForUnsortedSampleBuffers() 

Function

# CMBufferQueueGetCallbacksForUnsortedSampleBuffers()

Returns a pointer to a callback structure for unsorted sample buffers.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 6.0+

``` source
func CMBufferQueueGetCallbacksForUnsortedSampleBuffers() -> UnsafePointer
```

## See Also

### Inspecting Duration and Timing

func CMBufferQueueGetDuration(CMBufferQueue) -> CMTime

Gets the duration of a buffer queue.

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

