

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.RotationCoordinator
-  videoRotationAngleForHorizonLevelCapture 

Instance Property

# videoRotationAngleForHorizonLevelCapture

An angle the coordinator provides your app to apply to photos or videos it captures with the device so that they’re level relative to gravity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var videoRotationAngleForHorizonLevelCapture: CGFloat { get }
```

## Discussion

Your app can get immediate rotation angle updates from the rotation coordinator with key-value observation (KVO) of this property. The system calls key-value observation code on the main queue so that it has the same behavior as the videoRotationAngleForHorizonLevelPreview property.

Apps typically apply the property’s value to an AVCaptureConnection instance’s videoRotationAngle property, such as saving photos and videos with the correction rotation with AVCapturePhotoOutput and AVCaptureMovieFileOutput, respectively.

Alternatively, if your app uses an AVCaptureVideoDataOutput instance with an AVAssetWriter, such as for recording custom videos with effects, don’t rotate the video with AVCaptureConnection. Instead, set the rotation with an AVAssetWriterInput instance’s transform property, which alters the output file’s metadata. With this approach, video-playing apps apply the rotation during playback, which uses less energy than rotating each frame with the capture connection.

Note

Your app needs to convert the videoRotationAngleForHorizonLevelCapture value from degrees to radians for an asset writer input’s transform, which is a CGAffineTransform.

## See Also

### Compensating for a device’s rotation

var videoRotationAngleForHorizonLevelPreview: CGFloat

An angle the coordinator provides your app to apply to the preview layer so that it’s level relative to gravity.

