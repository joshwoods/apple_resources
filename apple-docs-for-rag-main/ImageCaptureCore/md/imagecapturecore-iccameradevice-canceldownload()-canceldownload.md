

- ImageCaptureCore
- ICCameraDevice
-  cancelDownload() 

Instance Method

# cancelDownload()

Cancels a download from the camera.

macOS 10.4+

``` source
func cancelDownload()
```

## See Also

### Downloading Files

struct ICDownloadOption

An option for downloading a file from the camera.

func requestDownloadFile(ICCameraFile, options: [ICDownloadOption : Any], downloadDelegate: any ICCameraDeviceDownloadDelegate, didDownloadSelector: Selector, contextInfo: UnsafeMutableRawPointer?)

Downloads a file from the camera.

protocol ICCameraDeviceDownloadDelegate

Methods for managing camera file downloads.

