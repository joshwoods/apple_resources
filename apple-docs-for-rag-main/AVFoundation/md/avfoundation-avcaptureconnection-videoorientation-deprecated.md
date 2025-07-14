

- AVFoundation
- AVCaptureConnection
-  videoOrientation Deprecated

Instance Property

# videoOrientation

An orientation that tells the connection how to rotate a video flowing through it.

iOS 4.0–17.0DeprecatediPadOS 4.0–17.0DeprecatedMac Catalyst 14.0–17.0DeprecatedmacOS 10.7–14.0Deprecated

``` source
var videoOrientation: AVCaptureVideoOrientation { get set }
```

Deprecated

See videoRotationAngle instead.

## Mentioned in 

Setting Up a Capture Session

## Discussion

The property only applies to a video connection.

If the value of isVideoOrientationSupported is true, you can set `videoOrientation` to rotate the video buffers consumed by the connection’s output. Setting `videoOrientation` doesn’t necessarily result in a physical rotation of video buffers. For example, a video connection to an AVCaptureMovieFileOutput object handles orientation using a QuickTime track matrix. A video connection to an AVCaptureStillImageOutput object handles orientation using EXIF tags.

AVCaptureVideoDataOutput clients may receive physically rotated pixel buffers in their captureOutput(_:didOutput:from:) delegate callback. The `AVCaptureVideoDataOutput` hardware accelerates the rotation operation and supports all four AVCaptureVideoOrientation modes. A client sets `videoOrientation` or isVideoMirrored on the video data output’s video AVCaptureConnection to request physical buffer rotation.

Important

Physically rotating buffers comes with a performance cost, so only request rotation when necessary. If you want to write rotated video to a movie file using AVAssetWriter, set the transform property on the AVAssetWriterInput instead.

## See Also

### Deprecated

var isVideoStabilizationEnabled: Bool

A Boolean value that indicates whether video stabilization is active for the connection.

Deprecated

var enablesVideoStabilizationWhenAvailable: Bool

A Boolean value that indicates whether the system enables video stabilization when it’s available.

Deprecated

var isVideoOrientationSupported: Bool

A Boolean value that indicates whether the connection supports changing the orientation of the video.

Deprecated

enum AVCaptureVideoOrientation

Constants indicating video orientation.

Deprecated

