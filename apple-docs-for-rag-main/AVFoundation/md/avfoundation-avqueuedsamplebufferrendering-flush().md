

- AVFoundation
- AVQueuedSampleBufferRendering
-  flush() 

Instance Method

# flush()

Discards all pending enqueued sample buffers.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func flush()
```

**Required**

## Discussion

It is not possible to determine which sample buffers have been decoded for video. The next frame passed to enqueue(_:) should be an IDR frame (also known as a key frame or sync sample).

