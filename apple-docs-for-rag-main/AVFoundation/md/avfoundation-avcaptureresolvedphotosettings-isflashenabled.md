

- AVFoundation
- AVCaptureResolvedPhotoSettings
-  isFlashEnabled 

Instance Property

# isFlashEnabled

A Boolean value indicating whether the camera flash fires for this capture.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
var isFlashEnabled: Bool { get }
```

## Discussion

This property corresponds to the AVCapturePhotoSettings property flashMode.

If you specify a flash mode of AVCaptureDevice.FlashMode.auto when requesting a capture, the device automatically chooses whether to use the flash based on the scene contents at the moment of capture. Therefore, you don’t know whether the flash will fire until right before the moment of capture. When the photo output calls your photoOutput(_:willBeginCaptureFor:) method (or other delegate methods that occur later in the capture process), you can use this property to determine whether a capture uses the flash.

Note

The flash can also become temporarily disabled if the device is too hot. In this case, the flash will not fire even if you specify a flash mode of AVCaptureDevice.FlashMode.on, and the resolved photo settings object passed to your AVCapturePhotoCaptureDelegate method has a isFlashEnabled value of false. To detect when the flash is temporarily disabled, key-value observe the isFlashAvailable property.

## See Also

### Examining Photo Capture Settings

var isRedEyeReductionEnabled: Bool

A Boolean value indicating whether the camera automatically reduces red-eye when capturing photos.

var isVirtualDeviceFusionEnabled: Bool

A Boolean value that specifies whether the system automatically uses virtual device image fusion.

var isFastCapturePrioritizationEnabled: Bool

A Boolean value that indicates whether the system uses fast capture prioritization when capturing the photo.

var isContentAwareDistortionCorrectionEnabled: Bool

A Boolean value that indicates whether the system applies content-aware distortion correction when capturing the photo.

var isStillImageStabilizationEnabled: Bool

A Boolean value indicating whether this capture uses image stabilization.

Deprecated

var isDualCameraFusionEnabled: Bool

A Boolean value indicating whether this capture combines image data from a dual camera.

Deprecated

