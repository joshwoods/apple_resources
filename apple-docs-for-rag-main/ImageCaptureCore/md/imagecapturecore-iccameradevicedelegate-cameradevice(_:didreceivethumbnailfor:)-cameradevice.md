

- ImageCaptureCore
- ICCameraDeviceDelegate
-  cameraDevice(\_:didReceiveThumbnailFor:) 

Instance Method

# cameraDevice(\_:didReceiveThumbnailFor:)

Tells the client when the requested thumbnail is available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.15DeprecatedvisionOS 1.0+

``` source
optional func cameraDevice(
    _ camera: ICCameraDevice,
    didReceiveThumbnailFor item: ICCameraItem
)
```

## Discussion

This method is deprecated. Use cameraDevice(_:didReceiveThumbnail:for:error:) instead.

## See Also

### Receiving Thumbnails

func cameraDevice(ICCameraDevice, didReceiveThumbnail: CGImage?, for: ICCameraItem, error: (any Error)?)

Tells the client when the requested thumbnail is available.

**Required**

func cameraDevice(ICCameraDevice, shouldGetThumbnailOf: ICCameraItem) -> Bool

Tells the client when the camera is about to execute queued requests for the thumbnail of a specific item.

