

- ImageCaptureCore
- ICCameraDevice
- ICCameraDeviceDownloadDelegate
-  didDownloadFile(\_:error:options:contextInfo:) 

Instance Method

# didDownloadFile(\_:error:options:contextInfo:)

Tells the delegate that the requested download has completed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.4+visionOS 1.0+

``` source
optional func didDownloadFile(
    _ file: ICCameraFile,
    error: (any Error)?,
    options: [String : Any] = [:],
    contextInfo: UnsafeMutableRawPointer?
)
```

## See Also

### Responding to Download Status

func didReceiveDownloadProgress(for: ICCameraFile, downloadedBytes: off_t, maxBytes: off_t)

Updates the delegate about the status of the download.

