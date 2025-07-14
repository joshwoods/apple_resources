

- AVFoundation
- AVQueuedSampleBufferRendering
-  stopRequestingMediaData() 

Instance Method

# stopRequestingMediaData()

Cancels any current requestMediaDataWhenReady(on:using:) call.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
func stopRequestingMediaData()
```

**Required**

## Discussion

Always pair a call to requestMediaDataWhenReady(on:using:) with this method. You can call this method from inside or outside of the requesting method’s block parameter.

## See Also

### Requesting Media

var isReadyForMoreMediaData: Bool

A Boolean value that indicates whether the receiver is able to accept more sample buffers.

**Required**

func enqueue(CMSampleBuffer)

Sends a sample buffer to the queue for rendering.

**Required**

func requestMediaDataWhenReady(on: dispatch_queue_t, using: () -> Void)

Tells the target to invoke a client-supplied block in order to gather sample buffers for playback.

**Required**

