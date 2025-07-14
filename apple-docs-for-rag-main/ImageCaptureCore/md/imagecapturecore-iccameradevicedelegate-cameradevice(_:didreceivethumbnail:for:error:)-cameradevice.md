

- ImageCaptureCore
- ICCameraDeviceDelegate
-  cameraDevice(\_:didReceiveThumbnail:for:error:) 

Instance Method

# cameraDevice(\_:didReceiveThumbnail:for:error:)

Tells the client when the requested thumbnail is available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func cameraDevice(
    _ camera: ICCameraDevice,
    didReceiveThumbnail thumbnail: CGImage?,
    for item: ICCameraItem,
    error: (any Error)?
)
```

**Required**

## See Also

### Receiving Thumbnails

func cameraDevice(ICCameraDevice, didReceiveThumbnailFor: ICCameraItem)

Tells the client when the requested thumbnail is available.

func cameraDevice(ICCameraDevice, shouldGetThumbnailOf: ICCameraItem) -> Bool

Tells the client when the camera is about to execute queued requests for the thumbnail of a specific item.

