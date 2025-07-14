

- WebKit
-  WKMediaCaptureState 

Enumeration

# WKMediaCaptureState

An enumeration that describes whether a media device, like a camera or microphone, is currently capturing audio or video.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
enum WKMediaCaptureState
```

## Topics

### Constants

case active

The media device is actively capturing audio or video.

case muted

The media device is muted, and not actively capturing audio or video.

case none

The media device is off.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Managing the microphone and camera

var cameraCaptureState: WKMediaCaptureState

An enumeration case that indicates whether the webpage is using the camera to capture images or video.

var microphoneCaptureState: WKMediaCaptureState

An enumeration case that indicates whether the webpage is using the microphone to capture audio.

func setCameraCaptureState(WKMediaCaptureState, completionHandler: (() -> Void)?)

Changes whether the webpage is using the camera to capture images or video.

func setMicrophoneCaptureState(WKMediaCaptureState, completionHandler: (() -> Void)?)

Changes whether the webpage is using the microphone to capture audio.

