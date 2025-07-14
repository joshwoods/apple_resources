

- WebKit
-  WKPermissionDecision 

Enumeration

# WKPermissionDecision

An enumeration of possible permission decisions for device resource access.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
enum WKPermissionDecision
```

## Topics

### Constants

case deny

Deny permission for the requested resource.

case grant

Grant permission for the requested resource.

case prompt

Prompt the user for permission for the requested resource.

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

enum WKMediaCaptureType

An enumeration listing the types of media devices that can capture audio, video, or both.

