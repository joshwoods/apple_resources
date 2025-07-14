

- ImageCaptureCore
- ICCameraDeviceDelegate
-  cameraDevice(\_:didReceiveMetadata:for:error:) 

Instance Method

# cameraDevice(\_:didReceiveMetadata:for:error:)

Tells the client when the metadata requested for an item on a camera is available.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
func cameraDevice(
    _ camera: ICCameraDevice,
    didReceiveMetadata metadata: [AnyHashable : Any]?,
    for item: ICCameraItem,
    error: (any Error)?
)
```

**Required**

## See Also

### Receiving Metadata

func cameraDevice(ICCameraDevice, shouldGetMetadataOf: ICCameraItem) -> Bool

Tells the client when the camera is about to execute queued requests for the metadata of a specific item.

func cameraDevice(ICCameraDevice, didReceiveMetadataFor: ICCameraItem)

Tells the client when the metadata requested for an item on a camera is available.

