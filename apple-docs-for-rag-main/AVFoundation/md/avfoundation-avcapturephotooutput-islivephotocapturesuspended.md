

- AVFoundation
- AVCapturePhotoOutput
-  isLivePhotoCaptureSuspended 

Instance Property

# isLivePhotoCaptureSuspended

A Boolean value that indicates whether Live Photo capture is currently in a suspended state.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isLivePhotoCaptureSuspended: Bool { get set }
```

## Discussion

By default, this property’s value is false. Set this value to true to stop any current Live Photo movie captures in progress. Doing this prevents recording additional actions in the Live Photo movie. For example, if you want to capture a still photo that makes a shutter sound, you can prevent recording that action.

When you change this value to true, the system trims any Live Photo movie captures in progress to the current time. Likewise, when you change this value from true to false, subsequent Live Photo movie captures won’t contain any earlier recordings.

By default, this property resets to false when the AVCaptureSession stops. You can prevent this behavior by setting preservesLivePhotoCaptureSuspendedOnSessionStop to true before stopping the session.

Important

Setting this property to true throws an invalidArgumentException if the isLivePhotoCaptureEnabled property’s value is false.

## See Also

### Configuring Live Photo Capture

var isLivePhotoCaptureSupported: Bool

A Boolean value that indicates whether the capture output currently supports Live Photo capture.

var isLivePhotoCaptureEnabled: Bool

A Boolean value that indicates whether to configure the capture pipeline for Live Photo capture.

var preservesLivePhotoCaptureSuspendedOnSessionStop: Bool

A Boolean value that indicates whether to preserve the suspended state of Live Photo capture when the session stops.

var isLivePhotoAutoTrimmingEnabled: Bool

A Boolean value that indicates whether to automatically trim Live Photo movie captures to avoid excessive movement.

var availableLivePhotoVideoCodecTypes: [AVVideoCodecType]

An array of video codecs currently available for Live Photo movie captures.

