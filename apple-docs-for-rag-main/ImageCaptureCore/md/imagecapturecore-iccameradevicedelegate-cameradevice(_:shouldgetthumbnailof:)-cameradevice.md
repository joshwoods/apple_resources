

- ImageCaptureCore
- ICCameraDeviceDelegate
-  cameraDevice(\_:shouldGetThumbnailOf:) 

Instance Method

# cameraDevice(\_:shouldGetThumbnailOf:)

Tells the client when the camera is about to execute queued requests for the thumbnail of a specific item.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
optional func cameraDevice(
    _ cameraDevice: ICCameraDevice,
    shouldGetThumbnailOf item: ICCameraItem
) -> Bool
```

## Discussion

If the request is no longer needed—for example, if the item is no longer displayed on the screen—the client can cancel sending a request to the camera, speeding up the execution queue.

## See Also

### Receiving Thumbnails

func cameraDevice(ICCameraDevice, didReceiveThumbnail: CGImage?, for: ICCameraItem, error: (any Error)?)

Tells the client when the requested thumbnail is available.

**Required**

func cameraDevice(ICCameraDevice, didReceiveThumbnailFor: ICCameraItem)

Tells the client when the requested thumbnail is available.

