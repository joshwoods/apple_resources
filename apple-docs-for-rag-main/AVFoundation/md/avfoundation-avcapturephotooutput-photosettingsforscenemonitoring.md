

- AVFoundation
- AVCapturePhotoOutput
-  photoSettingsForSceneMonitoring 

Instance Property

# photoSettingsForSceneMonitoring

A photo settings object that controls how the photo output detects and handles automatic flash and stabilization modes.

iOS 10.0+iPadOS 10.0+Mac Catalyst 14.0+tvOS 17.0+

``` source
@NSCopying
var photoSettingsForSceneMonitoring: AVCapturePhotoSettings? { get set }
```

## Discussion

Set the flashMode and isAutoStillImageStabilizationEnabled properties of this photo settings object to influence the values of the photo output’s scene monitoring properties (isFlashScene and isStillImageStabilizationScene). For example, if you set the flashMode property of this photo settings object to AVCaptureDevice.FlashMode.off, the photo output’s isFlashScene property reports false regardless of lighting conditions in the visible scene. If you set this photo settings object’s flashMode property to AVCaptureDevice.FlashMode.auto or AVCaptureDevice.FlashMode.on, the photo output’s isFlashScene property reverts to its default behavior of returning true or false based on the visible light level.

Note

There is some overlap in the light level ranges that benefit from still image stabilization and flash. If this photo settings object indicates that the scene should be monitored for both still image stabilization and flash, still image stabilization takes precedence, and the isFlashScene property becomes true at lower overall light levels.

The default value is an AVCapturePhotoSettings object with the following settings:

- flashMode: AVCaptureDevice.FlashMode.auto

- isAutoStillImageStabilizationEnabled: true

The photo output ignores all other properties of this photo settings object. To control other photo settings when requesting capture, create a photo settings object to pass to the capturePhoto(with:delegate:) method.

## See Also

### Monitoring the Visible Scene

var isFlashScene: Bool

A Boolean value indicating whether the scene currently being previewed by the camera warrants use of the flash.

