

- AVFoundation
- AVSampleBufferVideoRenderer
-  error 

Instance Property

# error

An object the describes the error that caused the rendering failure.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
var error: (any Error)? { get }
```

## Discussion

This value is `nil` by default. It only contains a valid error object when the status value is AVQueuedSampleBufferRenderingStatus.failed.

## See Also

### Inspecting the status

var status: AVQueuedSampleBufferRenderingStatus

A status value that indicates whether this object can enqueue and render sample buffers.

