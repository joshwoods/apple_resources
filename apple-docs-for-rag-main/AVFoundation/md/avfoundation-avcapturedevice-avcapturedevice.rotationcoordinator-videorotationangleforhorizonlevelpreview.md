

- AVFoundation
- AVCaptureDevice
- AVCaptureDevice.RotationCoordinator
-  videoRotationAngleForHorizonLevelPreview 

Instance Property

# videoRotationAngleForHorizonLevelPreview

An angle the coordinator provides your app to apply to the preview layer so that it’s level relative to gravity.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+

``` source
var videoRotationAngleForHorizonLevelPreview: CGFloat { get }
```

## Discussion

Your app can get immediate rotation angle updates from the rotation coordinator with key-value observation (KVO) for this property. You can immediately update your app’s UI from its key-value observation code because the rotation coordinator notifies your app on the main queue.

Important

Avoid unnecessary delays and visual artifacts by updating your app’s UI directly from an observer that monitors the property.

Apps typically apply the property’s value to an AVCaptureConnection instance’s videoRotationAngle property, such as displaying a camera preview with the correction for an AVCaptureVideoPreviewLayer instance.

Alternatively, if your app uses an AVCaptureVideoDataOutput instance to display a custom camera preview, such as with effects, don’t rotate the video with AVCaptureConnection. Instead, set the rotation in your CALayer instance’s transform property, such as with an AVSampleBufferDisplayLayer instance. This approach uses less energy than rotating each frame with the capture connection.

Note

Your app needs to convert the videoRotationAngleForHorizonLevelPreview value from degrees to radians for an asset writer layer’s transform, which is a CATransform3D.

## See Also

### Compensating for a device’s rotation

var videoRotationAngleForHorizonLevelCapture: CGFloat

An angle the coordinator provides your app to apply to photos or videos it captures with the device so that they’re level relative to gravity.

