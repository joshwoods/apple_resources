

- Foundation
- NSURLDownloadDelegate
-  download(\_:decideDestinationWithSuggestedFilename:) 

Instance Method

# download(\_:decideDestinationWithSuggestedFilename:)

The delegate receives this message when `download` has determined a suggested filename for the downloaded file.

macOS 10.2+

``` source
optional func download(
    _ download: NSURLDownload,
    decideDestinationWithSuggestedFilename filename: String
)
```

## Parameters 

`download`  

The URL download object sending the message.

`filename`  

The suggested filename for the download.

## Discussion

The suggested filename is either derived from the last path component of the URL and the MIME type or, if the download was encoded, from the encoding. If the delegate wishes to modify the path, it should send setDestination(_:allowOverwrite:) to `download`.

### Special Considerations

The delegate will not receive this message if `setDestination:allowOverwrite:` has already been called for the download.

## See Also

### Download Data and Responses

func downloadDidBegin(NSURLDownload)

Sent immediately after a download object begins a download.

func download(NSURLDownload, didCreateDestination: String)

Sent when the destination file is created.

func download(NSURLDownload, didReceive: URLResponse)

Sent when a download object has received sufficient load data to construct the NSURLResponse object for the download.

func download(NSURLDownload, didReceiveDataOfLength: Int)

Sent as a download object receives data incrementally.

func download(NSURLDownload, shouldDecodeSourceDataOfMIMEType: String) -> Bool

Sent when a download object determines that the downloaded file is encoded to inquire whether the file should be automatically decoded.

func download(NSURLDownload, willResumeWith: URLResponse, fromByte: Int64)

Sent when a download object has received a response from the server after attempting to resume a download.

func download(NSURLDownload, willSend: URLRequest, redirectResponse: URLResponse?) -> URLRequest?

Sent when the download object determines that it must change URLs in order to continue loading a request.

