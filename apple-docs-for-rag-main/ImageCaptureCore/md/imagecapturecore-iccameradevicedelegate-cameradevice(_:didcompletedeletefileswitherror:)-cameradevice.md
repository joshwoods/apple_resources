

- ImageCaptureCore
- ICCameraDeviceDelegate
-  cameraDevice(\_:didCompleteDeleteFilesWithError:) 

Instance Method

# cameraDevice(\_:didCompleteDeleteFilesWithError:)

Tells the client when the camera completes a delete operation.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
optional func cameraDevice(
    _ camera: ICCameraDevice,
    didCompleteDeleteFilesWithError error: (any Error)?
)
```

## Discussion

Initiate a delete operation using requestDeleteFiles(_:).

## See Also

### Removing Objects

func cameraDevice(ICCameraDevice, didRemove: [ICCameraItem])

Tells the client when objects are removed from the device.

**Required**

func cameraDevice(ICCameraDevice, didRemove: ICCameraItem)

Tells the client when an object is removed from the device.

