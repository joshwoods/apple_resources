

- AVFoundation
- AVCapturePhotoOutput
-  availableLivePhotoVideoCodecTypes 

Instance Property

# availableLivePhotoVideoCodecTypes

An array of video codecs currently available for Live Photo movie captures.

iOS 11.0+iPadOS 11.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var availableLivePhotoVideoCodecTypes: [AVVideoCodecType] { get }
```

## Discussion

By default, Live Photo capture encodes the movie portion of a Live Photo using the H.264 codec. To use a different codec, set the livePhotoVideoCodecType property of your photo settings object to one of the values in this array.

The system always presents its default video codec first. If you haven’t added the photo output to an AVCaptureSession with a video source, no codecs are available.

This property is key-value observable.

## See Also

### Configuring Live Photo Capture

var isLivePhotoCaptureSupported: Bool

A Boolean value that indicates whether the capture output currently supports Live Photo capture.

var isLivePhotoCaptureEnabled: Bool

A Boolean value that indicates whether to configure the capture pipeline for Live Photo capture.

var isLivePhotoCaptureSuspended: Bool

A Boolean value that indicates whether Live Photo capture is currently in a suspended state.

var preservesLivePhotoCaptureSuspendedOnSessionStop: Bool

A Boolean value that indicates whether to preserve the suspended state of Live Photo capture when the session stops.

var isLivePhotoAutoTrimmingEnabled: Bool

A Boolean value that indicates whether to automatically trim Live Photo movie captures to avoid excessive movement.

