

- AVFoundation
- AVSampleBufferVideoRenderer
-  status 

Instance Property

# status

A status value that indicates whether this object can enqueue and render sample buffers.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var status: AVQueuedSampleBufferRenderingStatus { get }
```

## Discussion

If the status is AVQueuedSampleBufferRenderingStatus.failed, check the value of the error property to determine the failure. To resume rendering sample buffers after a failure, you must first reset the status to AVQueuedSampleBufferRenderingStatus.unknown, which you do by invoking flush() on the video renderer.

This property is key-value observable.

## See Also

### Inspecting the status

var error: (any Error)?

An object the describes the error that caused the rendering failure.

