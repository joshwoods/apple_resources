

- AVFoundation
- AVCapturePhotoOutput
-  isLivePhotoCaptureEnabled 

Instance Property

# isLivePhotoCaptureEnabled

A Boolean value that indicates whether to configure the capture pipeline for Live Photo capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isLivePhotoCaptureEnabled: Bool { get set }
```

## Discussion

This value defaults to false. Changing this value while your session is running requires a lengthy reconfiguration of the capture render pipeline. If you intend to take any Live Photo captures, set this value to true before calling AVCaptureSession startRunning(). If you change this property while the session is running, in-progress Live Photo captures end immediately, unfulfilled photo requests cancel, and the video preview temporarily freezes.

You must enable this option before initiating a photo capture with the livePhotoMovieFileURL property of your photo settings object set to non-`nil`. However, after you’ve enabled this option, you can issue photo capture requests for both Live Photo captures and still photos.

## See Also

### Configuring Live Photo Capture

var isLivePhotoCaptureSupported: Bool

A Boolean value that indicates whether the capture output currently supports Live Photo capture.

var isLivePhotoCaptureSuspended: Bool

A Boolean value that indicates whether Live Photo capture is currently in a suspended state.

var preservesLivePhotoCaptureSuspendedOnSessionStop: Bool

A Boolean value that indicates whether to preserve the suspended state of Live Photo capture when the session stops.

var isLivePhotoAutoTrimmingEnabled: Bool

A Boolean value that indicates whether to automatically trim Live Photo movie captures to avoid excessive movement.

var availableLivePhotoVideoCodecTypes: [AVVideoCodecType]

An array of video codecs currently available for Live Photo movie captures.

