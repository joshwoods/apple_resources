

- AVFoundation
- AVCapturePhotoOutput
-  isHighResolutionCaptureEnabled Deprecated

Instance Property

# isHighResolutionCaptureEnabled

A Boolean value that specifies whether to configure the capture pipeline for high resolution still image capture.

iOS 10.0–16.0DeprecatediPadOS 10.0–16.0DeprecatedMac Catalyst 14.0–16.0DeprecatedmacOS 10.15–13.0Deprecated

``` source
var isHighResolutionCaptureEnabled: Bool { get set }
```

Deprecated

Use maxPhotoDimensions instead.

## Discussion

Some capture formats support output of still images at a resolution higher than the resolution they use for live preview and video capture (see the AVCaptureDevice.Format highResolutionStillImageDimensions property). Under some conditions, a capture session needs to set up its internal rendering pipeline differently to support high resolution still image capture.

If you intend to take high resolution still images at all, set this property to before calling the AVCaptureSession startRunning() method. Changing this property while the session is running requires a lengthy reconfiguration of the capture render pipeline: Live Photo captures in progress will end immediately, unfulfilled photo requests will abort, and video preview will temporarily freeze.

You must enable this option before initiating a photo capture with the isHighResolutionPhotoEnabled property of your photo settings object set to true. However, after you’ve enabled this option, you are free to issue photo capture requests with any isHighResolutionPhotoEnabled setting.

