

- AVFoundation
- AVSampleBufferAudioRenderer
-  error 

Instance Property

# error

The error that caused the renderer to no longer render sample buffers.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var error: (any Error)? { get }
```

## Discussion

The value of this property is nil unless the value of status is AVQueuedSampleBufferRenderingStatus.failed.

