

- WebKit
- WKUIDelegate
-  webView(\_:requestDeviceOrientationAndMotionPermissionFor:initiatedByFrame:decisionHandler:) 

Instance Method

# webView(\_:requestDeviceOrientationAndMotionPermissionFor:initiatedByFrame:decisionHandler:)

Determines whether a web resource, which the security origin object describes, can access the device’s orientation and motion.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    requestDeviceOrientationAndMotionPermissionFor origin: WKSecurityOrigin,
    initiatedByFrame frame: WKFrameInfo,
    decisionHandler: @escaping @MainActor (WKPermissionDecision) -> Void
)
```

## Parameters 

`webView`  

The web view requesting permission for orientation and motion information.

`origin`  

An object that identifies the host name, protocol, and port number for a web resource.

`frame`  

The frame that initiates the request in the web view.

`decisionHandler`  

A closure that you call from your delegate method. Pass the permission decision you determine to the closure.

## Discussion

If you don’t implement this method in your delegate, the system returns WKPermissionDecision.prompt.

## See Also

### Requesting permissions

func webView(WKWebView, requestMediaCapturePermissionFor: WKSecurityOrigin, initiatedByFrame: WKFrameInfo, type: WKMediaCaptureType, decisionHandler: (WKPermissionDecision) -> Void)

Determines whether a web resource, which the security origin object describes, can access to the device’s microphone audio and camera video.

enum WKPermissionDecision

An enumeration of possible permission decisions for device resource access.

enum WKMediaCaptureType

An enumeration listing the types of media devices that can capture audio, video, or both.

