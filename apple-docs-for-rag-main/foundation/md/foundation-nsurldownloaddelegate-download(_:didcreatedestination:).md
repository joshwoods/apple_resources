

- Foundation
- NSURLDownloadDelegate
-  download(\_:didCreateDestination:) 

Instance Method

# download(\_:didCreateDestination:)

Sent when the destination file is created.

macOS 10.2+

``` source
optional func download(
    _ download: NSURLDownload,
    didCreateDestination path: String
)
```

## Parameters 

`download`  

The URL download object sending the message.

`path`  

The path to the destination file.

## See Also

### Download Data and Responses

func download(NSURLDownload, decideDestinationWithSuggestedFilename: String)

The delegate receives this message when `download` has determined a suggested filename for the downloaded file.

func downloadDidBegin(NSURLDownload)

Sent immediately after a download object begins a download.

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

