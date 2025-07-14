

- AVFoundation
- AVQueuedSampleBufferRendering
-  requestMediaDataWhenReady(on:using:) 

Instance Method

# requestMediaDataWhenReady(on:using:)

Tells the target to invoke a client-supplied block in order to gather sample buffers for playback.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func requestMediaDataWhenReady(
    on queue: dispatch_queue_t,
    using block: @escaping () -> Void
)
```

**Required**

## Parameters 

`queue`  

The dispatch queue.

`block`  

A block that enqueues sample buffers until the receiver is no longer ready or there is no more data to supply.

## Discussion

When this method is called multiple times, only the last call is implemented. Pair each call to requestMediaDataWhenReady(on:using:) with a corresponding call to stopRequestingMediaData(). Releasing the `AVQueuedSampleBufferRendering` object without a call to `stopRequestingMediaData` results in undefined behavior.

## See Also

### Requesting Media

var isReadyForMoreMediaData: Bool

A Boolean value that indicates whether the receiver is able to accept more sample buffers.

**Required**

func enqueue(CMSampleBuffer)

Sends a sample buffer to the queue for rendering.

**Required**

func stopRequestingMediaData()

Cancels any current requestMediaDataWhenReady(on:using:) call.

**Required**

