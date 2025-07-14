

- AVFoundation
- AVCapturePhotoOutput
-  preservesLivePhotoCaptureSuspendedOnSessionStop 

Instance Property

# preservesLivePhotoCaptureSuspendedOnSessionStop

A Boolean value that indicates whether to preserve the suspended state of Live Photo capture when the session stops.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+

``` source
var preservesLivePhotoCaptureSuspendedOnSessionStop: Bool { get set }
```

## Discussion

This value defaults to false, which means that Live Photo capture resumes when the session stops. Set the value to true to save the state of the isLivePhotoCaptureSuspended property across session restarts.

## See Also

### Configuring Live Photo Capture

var isLivePhotoCaptureSupported: Bool

A Boolean value that indicates whether the capture output currently supports Live Photo capture.

var isLivePhotoCaptureEnabled: Bool

A Boolean value that indicates whether to configure the capture pipeline for Live Photo capture.

var isLivePhotoCaptureSuspended: Bool

A Boolean value that indicates whether Live Photo capture is currently in a suspended state.

var isLivePhotoAutoTrimmingEnabled: Bool

A Boolean value that indicates whether to automatically trim Live Photo movie captures to avoid excessive movement.

var availableLivePhotoVideoCodecTypes: [AVVideoCodecType]

An array of video codecs currently available for Live Photo movie captures.

