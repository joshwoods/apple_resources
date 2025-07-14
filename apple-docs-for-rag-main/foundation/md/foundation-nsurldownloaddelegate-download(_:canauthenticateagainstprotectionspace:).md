

- Foundation
- NSURLDownloadDelegate
-  download(\_:canAuthenticateAgainstProtectionSpace:) 

Instance Method

# download(\_:canAuthenticateAgainstProtectionSpace:)

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

macOS 10.2+

``` source
optional func download(
    _ connection: NSURLDownload,
    canAuthenticateAgainstProtectionSpace protectionSpace: URLProtectionSpace
) -> Bool
```

## Parameters 

`connection`  

The download sending the message.

`protectionSpace`  

The protection space that generates an authentication challenge.

## Discussion

This method is called before download(_:didReceive:), allowing the delegate to inspect a protection space before attempting to authenticate against it. By returning true, the delegate indicates that it can handle the form of authentication, which it does in the subsequent call to download(_:didReceive:). Not implementing this method is the same as returning false, in which case default authentication handling is used.

## See Also

### Download Authentication

func download(NSURLDownload, didCancel: URLAuthenticationChallenge)

Sent if an authentication challenge is canceled due to the protocol implementation encountering an error.

func download(NSURLDownload, didReceive: URLAuthenticationChallenge)

Sent when the URL download must authenticate a challenge in order to download the request.

func downloadShouldUseCredentialStorage(NSURLDownload) -> Bool

Sent to determine whether the URL loader should consult the credential storage to authenticate the download.

