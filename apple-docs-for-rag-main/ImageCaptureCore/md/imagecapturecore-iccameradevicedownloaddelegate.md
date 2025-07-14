

- ImageCaptureCore
-  ICCameraDeviceDownloadDelegate 

Protocol

# ICCameraDeviceDownloadDelegate

Methods for managing camera file downloads.

iOSiPadOSMac CatalystmacOSvisionOS

``` source
protocol ICCameraDeviceDownloadDelegate : NSObjectProtocol
```

## Topics

### Responding to Download Status

func didDownloadFile(ICCameraFile, error: (any Error)?, options: [String : Any], contextInfo: UnsafeMutableRawPointer?)

Tells the delegate that the requested download has completed.

func didReceiveDownloadProgress(for: ICCameraFile, downloadedBytes: off_t, maxBytes: off_t)

Updates the delegate about the status of the download.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Downloading Files

struct ICDownloadOption

An option for downloading a file from the camera.

func cancelDownload()

Cancels a download from the camera.

func requestDownloadFile(ICCameraFile, options: [ICDownloadOption : Any], downloadDelegate: any ICCameraDeviceDownloadDelegate, didDownloadSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Downloads a file from the camera.

