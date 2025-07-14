

- ImageCaptureCore
- ICCameraDeviceDelegate
-  cameraDevice(\_:didRemove:) 

Instance Method

# cameraDevice(\_:didRemove:)

Tells the client when objects are removed from the device.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func cameraDevice(
    _ camera: ICCameraDevice,
    didRemove items: [ICCameraItem]
)
```

**Required**

## Discussion

The objects in items are instances of the ICCameraFile class.

## See Also

### Removing Objects

func cameraDevice(ICCameraDevice, didCompleteDeleteFilesWithError: (any Error)?)

Tells the client when the camera completes a delete operation.

func cameraDevice(ICCameraDevice, didRemove: ICCameraItem)

Tells the client when an object is removed from the device.

