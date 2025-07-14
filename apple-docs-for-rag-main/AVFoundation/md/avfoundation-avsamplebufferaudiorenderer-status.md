

- AVFoundation
- AVSampleBufferAudioRenderer
-  status 

Instance Property

# status

The status of the audio renderer.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
var status: AVQueuedSampleBufferRenderingStatus { get }
```

## Discussion

A renderer begins with a status of AVQueuedSampleBufferRenderingStatus.unknown. As you add sample buffers to the queue for rendering, the renderer transitions to either AVQueuedSampleBufferRenderingStatus.rendering or AVQueuedSampleBufferRenderingStatus.failed.

If the status is `AVQueuedSampleBufferRenderingStatus.failed`, check the value of the renderer’s error property for information on the error encountered. This property is key value observable.

## See Also

### Determining Rendering Status

enum AVQueuedSampleBufferRenderingStatus

The statuses for sample buffer rendering.

