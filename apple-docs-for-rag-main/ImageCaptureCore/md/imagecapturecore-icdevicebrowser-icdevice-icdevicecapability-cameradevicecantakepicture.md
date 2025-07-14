

- ImageCaptureCore
- ICDeviceBrowser
- ICDevice
- ICDeviceCapability
-  cameraDeviceCanTakePicture 

Type Property

# cameraDeviceCanTakePicture

The capability for the client to request to take a picture while the camera is connected.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
static let cameraDeviceCanTakePicture: ICDeviceCapability
```

## Discussion

When this capability is available, the client can call requestTakePicture() to capture a picture.

## See Also

### Taking Pictures

static let cameraDeviceCanTakePictureUsingShutterReleaseOnCamera: ICDeviceCapability

The capability to capture a picture if the user presses the shutter release on the camera while the camera is connected.

