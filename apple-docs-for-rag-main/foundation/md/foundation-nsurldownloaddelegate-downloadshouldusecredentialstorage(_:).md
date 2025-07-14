

- Foundation
- NSURLDownloadDelegate
-  downloadShouldUseCredentialStorage(\_:) 

Instance Method

# downloadShouldUseCredentialStorage(\_:)

Sent to determine whether the URL loader should consult the credential storage to authenticate the download.

macOS 10.2+

``` source
optional func downloadShouldUseCredentialStorage(_ download: NSURLDownload) -> Bool
```

## Parameters 

`download`  

The connection sending the message.

## Discussion

This method is called before any attempt to authenticate is made. By returning false, the delegate tells the download not to consult the credential storage and makes itself responsible for providing credentials for any authentication challenges. Not implementing this method is the same as returing true. The delegate is free to consult the credential storage itself when it receives a download(_:didReceive:) message.

## See Also

### Download Authentication

func download(NSURLDownload, canAuthenticateAgainstProtectionSpace: URLProtectionSpace) -> Bool

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

func download(NSURLDownload, didCancel: URLAuthenticationChallenge)

Sent if an authentication challenge is canceled due to the protocol implementation encountering an error.

func download(NSURLDownload, didReceive: URLAuthenticationChallenge)

Sent when the URL download must authenticate a challenge in order to download the request.

