

- Foundation
-  NSURLDownloadDelegate 

Protocol

# NSURLDownloadDelegate

A protocol that URL download delegates implement to interact with a URL download request.

macOS 10.2+

``` source
protocol NSURLDownloadDelegate : NSObjectProtocol
```

## Overview

The NSURLDownloadDelegate protocol defines methods that allow an object to receive informational callbacks about the asynchronous load of a download’s URL request. Other delegate methods provide facilities that allow the delegate to customize the process of performing an asynchronous URL load.

Note that these delegate methods will be called on the thread that started the asynchronous load operation for the associated NSURLDownload object.

- A downloadDidBegin(_:) message will be sent to the delegate immediately upon starting the download.

- Zero or more download(_:willSend:redirectResponse:) messages will be sent to the delegate before any further messages are sent if it is determined that the download must redirect to a new location. The delegate can allow the redirect, modify the destination or deny the redirect.

- Zero or more download(_:didReceive:) messages will be sent to the delegate if it is necessary to authenticate in order to download the request and NSURLDownload does not already have authenticated credentials.

- Zero or more download(_:didCancel:) messages will be sent to the delegate if NSURLDownload cancels the authentication challenge due to encountering a protocol implementation error.

- Zero or more download(_:didReceive:) messages will be sent to the delegate before receiving a download(_:didReceiveDataOfLength:) message. The only case where download(_:didReceive:) is not sent to a delegate is when the protocol implementation encounters an error before a response could be created.

- Zero or more download(_:didReceiveDataOfLength:) messages will be sent before downloadDidFinish(_:) or download(_:didFailWithError:) is sent to the delegate.

- Zero or one download(_:decideDestinationWithSuggestedFilename:) will be sent to the delegate when sufficient information has been received to determine the suggested filename for the downloaded file. The delegate will not receive this message if setDestination(_:allowOverwrite:) has already been sent to the NSURLDownload instance.

- A download(_:didCreateDestination:) message will be sent to the delegate when the NSURLDownload instance creates the file on disk.

- If NSURLDownload determines that the downloaded file is in a format that it is able to decode (MacBinary, Binhex or gzip), the delegate will receive a download(_:shouldDecodeSourceDataOfMIMEType:). The delegate should return true to decode the data, false otherwise.

- Unless an NSURLDownload instance receives a cancel() message, the delegate will receive one and only one downloadDidFinish(_:) or download(_:didFailWithError:) message, but never both. In addition, once either of these messages are sent, the delegate will receive no further messages for the given NSURLDownload.

## Topics

### Download Authentication

func download(NSURLDownload, canAuthenticateAgainstProtectionSpace: URLProtectionSpace) -> Bool

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

func download(NSURLDownload, didCancel: URLAuthenticationChallenge)

Sent if an authentication challenge is canceled due to the protocol implementation encountering an error.

func download(NSURLDownload, didReceive: URLAuthenticationChallenge)

Sent when the URL download must authenticate a challenge in order to download the request.

func downloadShouldUseCredentialStorage(NSURLDownload) -> Bool

Sent to determine whether the URL loader should consult the credential storage to authenticate the download.

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

func download(NSURLDownload, willSend: URLRequest, redirectResponse: URLResponse?) -> URLRequest?

Sent when the download object determines that it must change URLs in order to continue loading a request.

### Download Completion

func download(NSURLDownload, didFailWithError: any Error)

Sent if the download fails or if an I/O error occurs when the file is written to disk.

func downloadDidFinish(NSURLDownload)

Sent when a download object has completed downloading successfully and has written its results to disk.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### URL Download

class NSURLDownload

An object that downloads a resource asynchronously and saves the data to a file.

