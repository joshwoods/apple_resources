

- Foundation
- NSURLDownloadDelegate
-  download(\_:willResumeWith:fromByte:) 

Instance Method

# download(\_:willResumeWith:fromByte:)

Sent when a download object has received a response from the server after attempting to resume a download.

macOS 10.2+

``` source
optional func download(
    _ download: NSURLDownload,
    willResumeWith response: URLResponse,
    fromByte startingByte: Int64
)
```

## Parameters 

`download`  

The URL download object sending the message.

`response`  

The URL response received from the server in response to an attempt to resume a download.

`startingByte`  

The location of the start of the resumed data, in bytes.

## See Also

### Download Data and Responses

func download(NSURLDownload, decideDestinationWithSuggestedFilename: String)

The delegate receives this message when `download` has determined a suggested filename for the downloaded file.

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

func download(NSURLDownload, willSend: URLRequest, redirectResponse: URLResponse?) -> URLRequest?

Sent when the download object determines that it must change URLs in order to continue loading a request.

