

- AVKit
- AVCaptureView
-  setSession(\_:showVideoPreview:showAudioPreview:) 

Instance Method

# setSession(\_:showVideoPreview:showAudioPreview:)

Sets the view’s capture session.

macOS 10.10+

``` source
@MainActor
func setSession(
    _ session: AVCaptureSession?,
    showVideoPreview: Bool,
    showAudioPreview: Bool
)
```

## Parameters 

`session`  

The capture session.

`showVideoPreview`  

A Boolean value that indicates whether the view displays a video preview. If true, the system adds, removes, or modifies capture inputs for video data based on device availability and user selection.

`showAudioPreview`  

A Boolean value that indicates whether the view shows an audio preview. If true, the system adds, removes, or modifies capture inputs for audio data based on device availability and user selection.

## Discussion

The view must show audio preview, video preview, or both. Furthermore, the view may modify the capture session, for example, to access media data for preview or when the user select a new capture source.

The capture view automatically starts and stops the default session. If you set a custom capture session on the view, you need to manually manage the session’s life cycle events.

## See Also

### Configuring the Capture Session

var session: AVCaptureSession?

The view’s associated capture session.

