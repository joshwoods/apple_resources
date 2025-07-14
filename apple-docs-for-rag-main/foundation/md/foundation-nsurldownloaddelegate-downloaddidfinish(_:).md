

- Foundation
- NSURLDownloadDelegate
-  downloadDidFinish(\_:) 

Instance Method

# downloadDidFinish(\_:)

Sent when a download object has completed downloading successfully and has written its results to disk.

macOS 10.2+

``` source
optional func downloadDidFinish(_ download: NSURLDownload)
```

## Parameters 

`download`  

The URL download object sending the message.

## Discussion

The delegate will receive no further messages for `download`.

## See Also

### Download Completion

func download(NSURLDownload, didFailWithError: any Error)

Sent if the download fails or if an I/O error occurs when the file is written to disk.

