

- Foundation
- NSURLConnectionDelegate
-  connection(\_:didReceive:) Deprecated

Instance Method

# connection(\_:didReceive:)

Sent when a connection must authenticate a challenge in order to download its request.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func connection(
    _ connection: NSURLConnection,
    didReceive challenge: URLAuthenticationChallenge
)
```

Deprecated

Use -connection:willSendRequestForAuthenticationChallenge: instead.

## Parameters 

`connection`  

The connection sending the message.

`challenge`  

The challenge that `connection` must authenticate in order to download its request.

## Discussion

This method gives the delegate the opportunity to determine the course of action taken for the challenge: provide credentials, continue without providing credentials, or cancel the authentication challenge and the download.

Note

This method is not called if the delegate implements the connection(_:willSendRequestFor:) method.

The delegate can determine the number of previous authentication challenges by sending the message previousFailureCount to `challenge`.

If the previous failure count is 0 and the value returned by proposedCredential is `nil`, the delegate can create a new NSURLCredential object, providing information specific to the type of credential, and send a use(_:for:) message to `[challenge sender]`, passing the credential and `challenge` as parameters. If proposedCredential is not `nil`, the value is a credential from the URL or the shared credential storage that can be provided to the user as feedback.

The delegate may decide to abandon further attempts at authentication at any time by sending `[challenge sender]` a continueWithoutCredential(for:) or a cancel(_:) message. The specific action is implementation dependent.

If the delegate implements this method, the download will suspend until `[challenge sender]` is sent one of the following messages: use(_:for:), continueWithoutCredential(for:) or cancel(_:).

If the delegate does not implement this method the default implementation is used. If a valid credential for the request is provided as part of the URL, or is available from the NSURLCredentialStorage the `[challenge sender]` is sent a use(_:for:) with the credential. If the challenge has no credential or the credentials fail to authorize access, then continueWithoutCredential(for:) is sent to `[challenge sender]` instead.

## See Also

### Related Documentation

func use(URLCredential, for: URLAuthenticationChallenge)

Attempt to use a given credential for a given authentication challenge.

**Required**

func continueWithoutCredential(for: URLAuthenticationChallenge)

Attempt to continue downloading a request without providing a credential for a given challenge.

**Required**

func cancel(URLAuthenticationChallenge)

Cancels a given authentication challenge.

**Required**

### Connection Authentication

func connection(NSURLConnection, willSendRequestFor: URLAuthenticationChallenge)

Tells the delegate that the connection will send a request for an authentication challenge.

func connection(NSURLConnection, canAuthenticateAgainstProtectionSpace: URLProtectionSpace) -> Bool

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

Deprecated

func connection(NSURLConnection, didCancel: URLAuthenticationChallenge)

Sent when a connection cancels an authentication challenge.

Deprecated

func connectionShouldUseCredentialStorage(NSURLConnection) -> Bool

Sent to determine whether the URL loader should use the credential storage for authenticating the connection.

