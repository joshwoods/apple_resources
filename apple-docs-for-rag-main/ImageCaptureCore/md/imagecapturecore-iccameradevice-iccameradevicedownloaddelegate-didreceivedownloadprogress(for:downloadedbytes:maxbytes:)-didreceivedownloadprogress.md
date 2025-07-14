

- ImageCaptureCore
- ICCameraDevice
- ICCameraDeviceDownloadDelegate
-  didReceiveDownloadProgress(for:downloadedBytes:maxBytes:) 

Instance Method

# didReceiveDownloadProgress(for:downloadedBytes:maxBytes:)

Updates the delegate about the status of the download.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
optional func didReceiveDownloadProgress(
    for file: ICCameraFile,
    downloadedBytes: off_t,
    maxBytes: off_t
)
```

## See Also

### Responding to Download Status

func didDownloadFile(ICCameraFile, error: (any Error)?, options: [String : Any], contextInfo: UnsafeMutableRawPointer?)

Tells the delegate that the requested download has completed.

