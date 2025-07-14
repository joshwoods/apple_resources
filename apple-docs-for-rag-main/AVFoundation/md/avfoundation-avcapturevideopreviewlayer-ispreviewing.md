

- AVFoundation
- AVCaptureVideoPreviewLayer
-  isPreviewing 

Instance Property

# isPreviewing

A Boolean value that indicates whether the layer is rendering video frames from its source.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isPreviewing: Bool { get }
```

## Discussion

A preview layer begins displaying content when you call the capture session’s startRunning() method. If you associate the layer with an instance of AVCaptureMultiCamSession, the system guarantees that all video preview layers display content by the time the blocking call to startRunning() or commitConfiguration() returns.

While a session is running, you may enable or disable a video preview layer’s connection to start or stop the flow of video to the layer. You may key-value observe the connection’s isEnabled property to observe this property changing, and synchronize any user interface changes to take place precisely when the video resumes rendering to the video preview layer.

## See Also

### Layer Configuration

var videoGravity: AVLayerVideoGravity

A value that indicates how the layer displays video content within its bounds.

