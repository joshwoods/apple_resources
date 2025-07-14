

- AVFoundation
- AVCaptureConnection
-  videoRotationAngle 

Instance Property

# videoRotationAngle

A rotation angle the connection applies to a video flowing through it.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var videoRotationAngle: CGFloat { get set }
```

## Discussion

Your app can set a video rotation angle that it gets from an AVCaptureDevice.RotationCoordinator instance’s videoRotationAngleForHorizonLevelCapture or videoRotationAngleForHorizonLevelPreview property. The rotation angle only applies to video or depth connections, similar to isVideoMirrored, and can be any angle that isVideoRotationAngleSupported(_:) returns true for.

Not all capture connections rotate each frame. For example, a video connection to an AVCaptureMovieFileOutput or AVCapturePhotoOutput instance applies a rotation with a QuickTime track matrix or with EXIF tags, respectively.

Capture connections to AVCaptureVideoDataOutput and AVCaptureDepthDataOutput instances rotate video frames they provide to their captureOutput(_:didOutput:from:) and depthDataOutput(_:didOutput:timestamp:connection:) delegate methods, respectively. Each AVCaptureVideoDataOutput instance uses hardware acceleration to rotate every frame.

Tip

Avoid potential performance issues by only rotating video with a capture connection when necessary.

You can rotate the video of a movie file you record with an AVAssetWriter instance by applying the rotation to an AVAssetWriterInput instance’s transform property. This approach avoids the performance costs that come with rotating each video frame.

Note

Your app needs to convert the videoRotationAngleForHorizonLevelCapture or videoRotationAngleForHorizonLevelPreview value from degrees to radians for transform properties.

## See Also

### Rotating a video

func isVideoRotationAngleSupported(CGFloat) -> Bool

Returns a Boolean value that indicates whether the connection supports a rotation angle.

