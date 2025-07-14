

- ImageCaptureCore
-  ICCameraDevice 

Class

# ICCameraDevice

An object that represents a camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
class ICCameraDevice
```

## Topics

### Reading Files

var contents: [ICCameraItem]?

All image, movie, and audio files stored on the camera, in an order that reflects the camera’s storage folder structure.

var mediaFiles: [ICCameraItem]?

All image, movie and audio files stored on the camera, without regard to the camera’s storage folder structure.

var contentCatalogPercentCompleted: Int

The percentage of the camera’s content that has been catalogued.

func files(ofType: String) -> [String]?

Returns an array of files of the selected type on the camera.

func requestReadData(from: ICCameraFile, atOffset: off_t, length: off_t, readDelegate: Any, didReadDataSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Asynchronously reads data of a specified length from a specified offset.

### Uploading Files

struct ICUploadOption

An option for uploading a file to the camera.

func requestUploadFile(URL, options: [ICUploadOption : Any], uploadDelegate: Any, didUploadSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Uploads a file to the camera.

Deprecated

### Downloading Files

struct ICDownloadOption

An option for downloading a file from the camera.

func cancelDownload()

Cancels a download from the camera.

func requestDownloadFile(ICCameraFile, options: [ICDownloadOption : Any], downloadDelegate: any ICCameraDeviceDownloadDelegate, didDownloadSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Downloads a file from the camera.

protocol ICCameraDeviceDownloadDelegate

Methods for managing camera file downloads.

### Deleting Files

var isLocked: Bool

A Boolean value indicating whether the device is locked, preventing deletion of any asset.

struct ICDeleteResult

The result of a deletion request.

struct ICDeleteError

An error resulting from a deletion request.

func requestDeleteFiles([ICCameraItem])

Deletes files from the camera.

func requestDeleteFiles([ICCameraItem], deleteFailed: ([ICDeleteError : ICCameraItem]) -> Void, completion: ([ICDeleteResult : [ICCameraItem]], (any Error)?) -> Void) -> Progress?

Deletes files from the camera, with the ability to catch failures and execute a completion block.

func cancelDelete()

Cancels the current delete operation.

### Taking Pictures

var tetheredCaptureEnabled: Bool

A Boolean value indicating whether tethered capture is enabled on the camera.

var ptpEventHandler: (Data) -> Void

A closure for handling PTP event packets.

func requestEnableTethering()

Enables tethered capture if the camera has the capability to take pictures while connected.

Deprecated

func requestTakePicture()

Captures a new image using the camera.

func requestSendPTPCommand(Data, outData: Data?, sendCommandDelegate: Any, didSendCommand: Selector, contextInfo: UnsafeMutableRawPointer?)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestSendPTPCommand(Data, outData: Data?, completion: (Data, Data, (any Error)?) -> Void)

Sends a Picture Transfer Protocol (PTP) command to a camera asynchronously.

func requestDisableTethering()

Disables tethered capture on the camera.

Deprecated

### Inspecting the Battery Charge Level

var batteryLevelAvailable: Bool

A Boolean value that indicates whether the battery charge level is available.

var batteryLevel: Int

The battery charge level.

### Synchronizing the Clock

var timeOffset: TimeInterval

The time offset, in seconds, between the camera’s clock and the computer’s clock.

func requestSyncClock()

Synchronizes the camera’s clock with the computer’s clock.

### Detecting Apple Devices

var isAccessRestrictedAppleDevice: Bool

A Boolean value indicating whether the device is an Apple device, passcode-locked, and connected to an untrusted host.

var iCloudPhotosEnabled: Bool

A Boolean value indicating whether the iCloud Photo Library is enabled on the device.

### Detecting Mass Storage Devices

var mountPoint: String?

The file system mount point for a camera using the mass storage transport type.

### Removing a Device

var isEjectable: Bool

A Boolean value indicating whether the device can be ‘soft’ removed or disconnected.

### Instance Properties

var mediaPresentation: ICMediaPresentation

## Relationships

### Inherits From

- ICDevice

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Cameras

protocol ICCameraDeviceDelegate

Methods for detecting cameras, getting metadata and thumbnails, handling access and capability changes, and performing other actions on connected cameras.

class ICCameraItem

An abstract class that represents a camera item.

class ICCameraFile

An object that represents a file on a camera.

class ICCameraFolder

An object that represents a folder on a camera.

