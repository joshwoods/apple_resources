

- AVFoundation
- AVCapturePhotoOutput
-  maxPhotoDimensions 

Instance Property

# maxPhotoDimensions

The maximum resolution of the requested photo.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 17.0+

``` source
var maxPhotoDimensions: CMVideoDimensions { get set }
```

## Discussion

Set a value for this property to request images up to the specified dimensions. Images that a photo output returns may be smaller than the dimensions, but are never be larger. Once set, you can request images with any valid maximum photo dimensions by setting maxPhotoDimensions on AVCapturePhotoSettings on a per photo basis.

The dimensions you set must match one returned by supportedMaxPhotoDimensions for the current active format.

Tip

Changing this property may trigger a lengthy reconfiguration of the capture pipeline, so set this value before calling startRunning() on the capture session.

