

- Foundation
- NSURLDownloadDelegate
-  download(\_:didFailWithError:) 

Instance Method

# download(\_:didFailWithError:)

Sent if the download fails or if an I/O error occurs when the file is written to disk.

macOS 10.2+

``` source
optional func download(
    _ download: NSURLDownload,
    didFailWithError error: any Error
)
```

## Parameters 

`download`  

The URL download object sending the message.

`error`  

The error that caused the failure of the download.

## Discussion

Any partially downloaded file will be deleted.

### Special Considerations

Once the delegate receives this message, it will receive no further messages for `download`.

## See Also

### Download Completion

func downloadDidFinish(NSURLDownload)

Sent when a download object has completed downloading successfully and has written its results to disk.

