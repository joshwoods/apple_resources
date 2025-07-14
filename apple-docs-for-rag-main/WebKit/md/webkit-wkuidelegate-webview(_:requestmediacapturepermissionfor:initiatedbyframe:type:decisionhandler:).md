

- WebKit
- WKUIDelegate
-  webView(\_:requestMediaCapturePermissionFor:initiatedByFrame:type:decisionHandler:) 

Instance Method

# webView(\_:requestMediaCapturePermissionFor:initiatedByFrame:type:decisionHandler:)

Determines whether a web resource, which the security origin object describes, can access to the device’s microphone audio and camera video.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    requestMediaCapturePermissionFor origin: WKSecurityOrigin,
    initiatedByFrame frame: WKFrameInfo,
    type: WKMediaCaptureType,
    decisionHandler: @escaping @MainActor (WKPermissionDecision) -> Void
)
```

``` source
@MainActor
optional func webView(
    _ webView: WKWebView,
    decideMediaCapturePermissionsFor origin: WKSecurityOrigin,
    initiatedBy frame: WKFrameInfo,
    type: WKMediaCaptureType
) async -> WKPermissionDecision
```

## Parameters 

`webView`  

The web view requesting permission for microphone audio and camera video.

`origin`  

An object that identifies the host name, protocol, and port number for a web resource.

`frame`  

The frame that initiates the request in the web view.

`type`  

An enumeration case representing a type of media capture device, like a microphone or camera.

`decisionHandler`  

A closure that you call from your delegate method. Pass the permission decision you determine to the closure.

## Discussion

If you don’t implement this method in your delegate, the system returns WKPermissionDecision.prompt.

## See Also

### Requesting permissions

func webView(WKWebView, requestDeviceOrientationAndMotionPermissionFor: WKSecurityOrigin, initiatedByFrame: WKFrameInfo, decisionHandler: (WKPermissionDecision) -> Void)

Determines whether a web resource, which the security origin object describes, can access the device’s orientation and motion.

enum WKPermissionDecision

An enumeration of possible permission decisions for device resource access.

enum WKMediaCaptureType

An enumeration listing the types of media devices that can capture audio, video, or both.

