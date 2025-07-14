

- Foundation
- NSURLDownloadDelegate
-  download(\_:willSend:redirectResponse:) 

Instance Method

# download(\_:willSend:redirectResponse:)

Sent when the download object determines that it must change URLs in order to continue loading a request.

macOS 10.2+

``` source
optional func download(
    _ download: NSURLDownload,
    willSend request: URLRequest,
    redirectResponse: URLResponse?
) -> URLRequest?
```

## Parameters 

`download`  

The URL download object sending the message.

`request`  

The proposed redirected request. The delegate should inspect the redirected request to verify that it meets its needs, and create a copy with new attributes to return to the connection if necessary.

`redirectResponse`  

The URL response that caused the redirect. May be `nil` in cases where this method is not being sent as a result of involving the delegate in redirect processing.

## Return Value

The actual URL request to use in light of the redirection response. The delegate may copy and modify `request` as necessary to change its attributes, return `request` unmodified, or return `nil`.

## Discussion

If the delegate wishes to cancel the redirect, it should call the `download` object’s cancel() method. Alternatively, the delegate method can return `nil` to cancel the redirect, and the download will continue to process. This has special relevance in the case where `redirectResponse` is not `nil`. In this case, any data that is loaded for the download will be sent to the delegate, and the delegate will receive a downloadDidFinish(_:) or download(_:didFailWithError:) message, as appropriate.

### Special Considerations

The delegate can receive this message as a result of transforming a request’s URL to its canonical form, or for protocol-specific reasons, such as an HTTP redirect. The delegate implementation should be prepared to receive this message multiple times.

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

func download(NSURLDownload, willResumeWith: URLResponse, fromByte: Int64)

Sent when a download object has received a response from the server after attempting to resume a download.

