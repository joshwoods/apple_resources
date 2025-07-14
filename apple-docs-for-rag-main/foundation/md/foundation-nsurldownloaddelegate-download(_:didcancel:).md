

- Foundation
- NSURLDownloadDelegate
-  download(\_:didCancel:) 

Instance Method

# download(\_:didCancel:)

Sent if an authentication challenge is canceled due to the protocol implementation encountering an error.

macOS 10.2+

``` source
optional func download(
    _ download: NSURLDownload,
    didCancel challenge: URLAuthenticationChallenge
)
```

## Parameters 

`download`  

The URL download object sending the message.

`challenge`  

The authentication challenge that caused the download object to cancel the download.

## Discussion

If the delegate receives this message the download will fail and the delegate will receive a download(_:didFailWithError:) message.

## See Also

### Download Authentication

func download(NSURLDownload, canAuthenticateAgainstProtectionSpace: URLProtectionSpace) -> Bool

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

func download(NSURLDownload, didReceive: URLAuthenticationChallenge)

Sent when the URL download must authenticate a challenge in order to download the request.

func downloadShouldUseCredentialStorage(NSURLDownload) -> Bool

Sent to determine whether the URL loader should consult the credential storage to authenticate the download.

