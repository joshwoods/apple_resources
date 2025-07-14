

- WebKit
- WKWebView
-  cameraCaptureState 

Instance Property

# cameraCaptureState

An enumeration case that indicates whether the webpage is using the camera to capture images or video.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor
var cameraCaptureState: WKMediaCaptureState { get }
```

## See Also

### Managing the microphone and camera

var microphoneCaptureState: WKMediaCaptureState

An enumeration case that indicates whether the webpage is using the microphone to capture audio.

func setCameraCaptureState(WKMediaCaptureState, completionHandler: (() -> Void)?)

Changes whether the webpage is using the camera to capture images or video.

func setMicrophoneCaptureState(WKMediaCaptureState, completionHandler: (() -> Void)?)

Changes whether the webpage is using the microphone to capture audio.

enum WKMediaCaptureState

An enumeration that describes whether a media device, like a camera or microphone, is currently capturing audio or video.

