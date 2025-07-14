

- AVKit
- AVCaptureView
-  session 

Instance Property

# session

The view’s associated capture session.

macOS 10.10+

``` source
@MainActor
var session: AVCaptureSession? { get }
```

## Discussion

This property’s default value is a capture session configured for movie file recordings of audio and video data. Use the setSession(_:showVideoPreview:showAudioPreview:) method to provide a custom capture session. Modifying the capture session changes its visual representation in the view.

## See Also

### Configuring the Capture Session

func setSession(AVCaptureSession?, showVideoPreview: Bool, showAudioPreview: Bool)

Sets the view’s capture session.

