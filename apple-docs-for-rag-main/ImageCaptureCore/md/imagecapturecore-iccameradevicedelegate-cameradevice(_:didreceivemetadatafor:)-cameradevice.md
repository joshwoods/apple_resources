

- ImageCaptureCore
- ICCameraDeviceDelegate
-  cameraDevice(\_:didReceiveMetadataFor:) 

Instance Method

# cameraDevice(\_:didReceiveMetadataFor:)

Tells the client when the metadata requested for an item on a camera is available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1–13.1DeprecatedmacOS 10.4–10.15DeprecatedvisionOS 1.0+

``` source
optional func cameraDevice(
    _ camera: ICCameraDevice,
    didReceiveMetadataFor item: ICCameraItem
)
```

## See Also

### Receiving Metadata

func cameraDevice(ICCameraDevice, didReceiveMetadata: [AnyHashable : Any]?, for: ICCameraItem, error: (any Error)?)

Tells the client when the metadata requested for an item on a camera is available.

**Required**

func cameraDevice(ICCameraDevice, shouldGetMetadataOf: ICCameraItem) -> Bool

Tells the client when the camera is about to execute queued requests for the metadata of a specific item.

