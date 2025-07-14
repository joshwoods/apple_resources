

- ImageCaptureCore
- ICCameraDevice
-  requestDownloadFile(\_:options:downloadDelegate:didDownloadSelector:contextInfo:) 

Instance Method

# requestDownloadFile(\_:options:downloadDelegate:didDownloadSelector:contextInfo:)

Downloads a file from the camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
func requestDownloadFile(
    _ file: ICCameraFile,
    options: [ICDownloadOption : Any] = [:],
    downloadDelegate: any ICCameraDeviceDownloadDelegate,
    didDownloadSelector selector: Selector,
    contextInfo: UnsafeMutableRawPointer?
)
```

## Discussion

Once this request completes, didDownloadFile(_:error:options:contextInfo:) is called on the `downloadDelegate`.

## See Also

### Downloading Files

struct ICDownloadOption

An option for downloading a file from the camera.

func cancelDownload()

Cancels a download from the camera.

protocol ICCameraDeviceDownloadDelegate

Methods for managing camera file downloads.

