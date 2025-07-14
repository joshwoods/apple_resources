

- Foundation
- NSURLDownloadDelegate
-  download(\_:didReceive:) 

Instance Method

# download(\_:didReceive:)

Sent when the URL download must authenticate a challenge in order to download the request.

macOS 10.2+

``` source
optional func download(
    _ download: NSURLDownload,
    didReceive challenge: URLAuthenticationChallenge
)
```

## Parameters 

`download`  

The URL download object sending the message.

`challenge`  

The URL authentication challenge that must be authenticated in order to download the request.

## Discussion

This method gives the delegate the opportunity to determine the course of action taken for the challenge: provide credentials, continue without providing credentials or cancel the authentication challenge and the download.

The delegate can determine the number of previous authentication challenges by sending the message previousFailureCount to `challenge`.

If the previous failure count is 0 and the value returned by proposedCredential is `nil`, the delegate can create a new NSURLCredential object, providing information specific to the type of credential, and send a use(_:for:) message to `[challenge sender]`, passing the credential and `challenge` as parameters. If proposedCredential is not `nil`, the value is a credential from the URL or the shared credential storage that can be provided to the user as feedback.

The delegate may decide to abandon further attempts at authentication at any time by sending `[challenge sender]` a continueWithoutCredential(for:) or a cancel(_:) message. The specific action is implementation dependent.

If the delegate implements this method, the download will suspend until `[challenge sender]` is sent one of the following messages: use(_:for:), continueWithoutCredential(for:) or cancel(_:).

If the delegate does not implement this method the default implementation is used. If a valid credential for the request is provided as part of the URL, or is available from the NSURLCredentialStorage the `[challenge sender]` is sent a use(_:for:) with the credential. If the challenge has no credential or the credentials fail to authorize access, then continueWithoutCredential(for:) is sent to `[challenge sender]` instead.

## See Also

### Download Authentication

func download(NSURLDownload, canAuthenticateAgainstProtectionSpace: URLProtectionSpace) -> Bool

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

func download(NSURLDownload, didCancel: URLAuthenticationChallenge)

Sent if an authentication challenge is canceled due to the protocol implementation encountering an error.

func downloadShouldUseCredentialStorage(NSURLDownload) -> Bool

Sent to determine whether the URL loader should consult the credential storage to authenticate the download.

