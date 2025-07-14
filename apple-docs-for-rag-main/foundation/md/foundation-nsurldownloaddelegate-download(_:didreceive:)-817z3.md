

- Foundation
- NSURLDownloadDelegate
-  download(\_:didReceive:) 

Instance Method

# download(\_:didReceive:)

Sent when a download object has received sufficient load data to construct the NSURLResponse object for the download.

macOS 10.2+

``` source
optional func download(
    _ download: NSURLDownload,
    didReceive response: URLResponse
)
```

## Parameters 

`download`  

The URL download object sending the message.

`response`  

The URL response object received as part of the download. `response` is immutable and will not be modified after this method is called.

## Discussion

In some rare cases, multiple responses may be received for a single download. In this case, the client should assume that each new response resets the download progress to 0 and should check the new response for the expected content length.

## See Also

### Download Data and Responses

func download(NSURLDownload, decideDestinationWithSuggestedFilename: String)

The delegate receives this message when `download` has determined a suggested filename for the downloaded file.

func downloadDidBegin(NSURLDownload)

Sent immediately after a download object begins a download.

func download(NSURLDownload, didCreateDestination: String)

Sent when the destination file is created.

func download(NSURLDownload, didReceiveDataOfLength: Int)

Sent as a download object receives data incrementally.

func download(NSURLDownload, shouldDecodeSourceDataOfMIMEType: String) -> Bool

Sent when a download object determines that the downloaded file is encoded to inquire whether the file should be automatically decoded.

func download(NSURLDownload, willResumeWith: URLResponse, fromByte: Int64)

Sent when a download object has received a response from the server after attempting to resume a download.

func download(NSURLDownload, willSend: URLRequest, redirectResponse: URLResponse?) -> URLRequest?

Sent when the download object determines that it must change URLs in order to continue loading a request.

