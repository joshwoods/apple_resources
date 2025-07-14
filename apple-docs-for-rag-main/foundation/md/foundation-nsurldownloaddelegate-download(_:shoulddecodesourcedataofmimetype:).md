

- Foundation
- NSURLDownloadDelegate
-  download(\_:shouldDecodeSourceDataOfMIMEType:) 

Instance Method

# download(\_:shouldDecodeSourceDataOfMIMEType:)

Sent when a download object determines that the downloaded file is encoded to inquire whether the file should be automatically decoded.

macOS 10.2+

``` source
optional func download(
    _ download: NSURLDownload,
    shouldDecodeSourceDataOfMIMEType encodingType: String
) -> Bool
```

## Parameters 

`download`  

The URL download object sending the message.

`encodingType`  

The type of encoding used by the downloaded file. The supported encoding formats are MacBinary (`"application/macbinary"`), Binhex (`"application/mac-binhex40"`) and gzip (`"application/gzip"`).

## Return Value

true to decode the file, false otherwise.

## Discussion

The delegate may receive this message more than once if the file has been encoded multiple times. This method is not called if the downloaded file is not encoded.

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

func download(NSURLDownload, willResumeWith: URLResponse, fromByte: Int64)

Sent when a download object has received a response from the server after attempting to resume a download.

func download(NSURLDownload, willSend: URLRequest, redirectResponse: URLResponse?) -> URLRequest?

Sent when the download object determines that it must change URLs in order to continue loading a request.

