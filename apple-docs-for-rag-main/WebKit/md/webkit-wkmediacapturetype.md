

- WebKit
-  WKMediaCaptureType 

Enumeration

# WKMediaCaptureType

An enumeration listing the types of media devices that can capture audio, video, or both.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
enum WKMediaCaptureType
```

## Topics

### Constants

case camera

A media device that can capture video.

case cameraAndMicrophone

A media device or devices that can capture audio and video.

case microphone

A media device that can capture audio.

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

### Requesting permissions

func webView(WKWebView, requestDeviceOrientationAndMotionPermissionFor: WKSecurityOrigin, initiatedByFrame: WKFrameInfo, decisionHandler: (WKPermissionDecision) -> Void)

Determines whether a web resource, which the security origin object describes, can access the device’s orientation and motion.

func webView(WKWebView, requestMediaCapturePermissionFor: WKSecurityOrigin, initiatedByFrame: WKFrameInfo, type: WKMediaCaptureType, decisionHandler: (WKPermissionDecision) -> Void)

Determines whether a web resource, which the security origin object describes, can access to the device’s microphone audio and camera video.

enum WKPermissionDecision

An enumeration of possible permission decisions for device resource access.

