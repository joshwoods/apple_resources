

- ImageCaptureCore
-  ICCameraDeviceDelegate 

Protocol

# ICCameraDeviceDelegate

Methods for detecting cameras, getting metadata and thumbnails, handling access and capability changes, and performing other actions on connected cameras.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
protocol ICCameraDeviceDelegate : ICDeviceDelegate
```

## Topics

### Determining Device Readiness

func deviceDidBecomeReady(withCompleteContentCatalog: ICCameraDevice)

Tells the client that the camera device is done enumerating its content and is ready to receive requests.

**Required**

### Adding Objects

func cameraDevice(ICCameraDevice, didAdd: [ICCameraItem])

Tells the client when objects are added to the device.

**Required**

func cameraDevice(ICCameraDevice, didAdd: ICCameraItem)

Tells the client when an object is added to the device.

### Removing Objects

func cameraDevice(ICCameraDevice, didRemove: [ICCameraItem])

Tells the client when objects are removed from the device.

**Required**

func cameraDevice(ICCameraDevice, didCompleteDeleteFilesWithError: (any Error)?)

Tells the client when the camera completes a delete operation.

func cameraDevice(ICCameraDevice, didRemove: ICCameraItem)

Tells the client when an object is removed from the device.

### Renaming Objects

func cameraDevice(ICCameraDevice, didRenameItems: [ICCameraItem])

Tells the client when one or more objects are renamed on the device.

**Required**

### Receiving Metadata

func cameraDevice(ICCameraDevice, didReceiveMetadata: [AnyHashable : Any]?, for: ICCameraItem, error: (any Error)?)

Tells the client when the metadata requested for an item on a camera is available.

**Required**

func cameraDevice(ICCameraDevice, shouldGetMetadataOf: ICCameraItem) -> Bool

Tells the client when the camera is about to execute queued requests for the metadata of a specific item.

func cameraDevice(ICCameraDevice, didReceiveMetadataFor: ICCameraItem)

Tells the client when the metadata requested for an item on a camera is available.

### Receiving Thumbnails

func cameraDevice(ICCameraDevice, didReceiveThumbnail: CGImage?, for: ICCameraItem, error: (any Error)?)

Tells the client when the requested thumbnail is available.

**Required**

func cameraDevice(ICCameraDevice, didReceiveThumbnailFor: ICCameraItem)

Tells the client when the requested thumbnail is available.

func cameraDevice(ICCameraDevice, shouldGetThumbnailOf: ICCameraItem) -> Bool

Tells the client when the camera is about to execute queued requests for the thumbnail of a specific item.

### Responding to Capability Changes

func cameraDeviceDidChangeCapability(ICCameraDevice)

Tells the client when a capability of a camera changes.

**Required**

### Responding to Access Restrictions

func cameraDeviceDidEnableAccessRestriction(ICDevice)

Tells the client when an Apple device has been locked, and media is unavailable until the restriction has been removed.

**Required**

func cameraDeviceDidRemoveAccessRestriction(ICDevice)

Tells the client when an Apple device has been unlocked, paired to the host, and media is available.

**Required**

### Responding to PTP Events

func cameraDevice(ICCameraDevice, didReceivePTPEvent: Data)

Tells the client about a PTP event.

**Required**

## Relationships

### Inherits From

- ICDeviceDelegate
- NSObjectProtocol

## See Also

### Cameras

class ICCameraDevice

An object that represents a camera.

class ICCameraItem

An abstract class that represents a camera item.

class ICCameraFile

An object that represents a file on a camera.

class ICCameraFolder

An object that represents a folder on a camera.

