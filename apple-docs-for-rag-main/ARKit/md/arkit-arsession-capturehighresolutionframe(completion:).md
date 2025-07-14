

- ARKit
- ARSession
-  captureHighResolutionFrame(completion:) 

Instance Method

# captureHighResolutionFrame(completion:)

Requests a frame outside of the normal frequency that contains a high-resolution captured image.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func captureHighResolutionFrame(completion: @escaping (ARFrame?, (any Error)?) -> Void)
```

``` source
func captureHighResolutionFrame() async throws -> ARFrame
```

## Parameters 

`completion`  

Code you provide that the framework runs after attempting to generate the frame.

## Discussion

If the function succeeds, the completion handler’s frame contains a high quality, high resolution capturedImage.

In the event of failure, the completion block receives a non-`nil` error object. A call may fail if a previous request for a high resolution capture hasn’t completed yet, or an underlying problem occurs in the system’s capture pipeline. You can identify the failure reason in either case by checking for highResolutionFrameCaptureInProgress or highResolutionFrameCaptureFailed, respectively.

ARKit populates the frame’s properties other than pixel data, including pose information, anchors, and frame semantics. The system provides the frame to your completion handler asynchronously.

You can call this function at any time during a session. The system delivers a high-resolution frame out-of-band, which means that it doesn’t affect the other frames that the session receives at a regular interval, such as currentFrame or the frame argument to session(_:didUpdate:).

For the highest resolution captured image, choose a non-binned videoFormat in your session’s configuration. You can call recommendedVideoFormatForHighResolutionFrameCapturing to select the best option for you.

For the highest resolution still images, choose a videoFormat among your configuration’s supportedVideoFormats that returns `true` for isRecommendedForHighResolutionFrameCapturing. If your app doesn’t have specific resolution requirements, you can use the framework-recommended format that recommendedVideoFormatForHighResolutionFrameCapturing returns.

## See Also

### Accessing the camera frame

var currentFrame: ARFrame?

The most recent still frame captured by the active camera feed, including ARKit’s interpretation of it.

class ARFrame

A video image captured as part of a session with position-tracking information.

