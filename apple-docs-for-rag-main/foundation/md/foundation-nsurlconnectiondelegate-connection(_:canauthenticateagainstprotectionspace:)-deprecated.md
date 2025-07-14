

- Foundation
- NSURLConnectionDelegate
-  connection(\_:canAuthenticateAgainstProtectionSpace:) Deprecated

Instance Method

# connection(\_:canAuthenticateAgainstProtectionSpace:)

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

iOS 3.0–8.0DeprecatediPadOS 3.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.6–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func connection(
    _ connection: NSURLConnection,
    canAuthenticateAgainstProtectionSpace protectionSpace: URLProtectionSpace
) -> Bool
```

Deprecated

Use -connection:willSendRequestForAuthenticationChallenge: instead.

## Parameters 

`connection`  

The connection sending the message.

`protectionSpace`  

The protection space that generates an authentication challenge.

## Return Value

true if the delegate if able to respond to a protection space’s form of authentication, otherwise false.

## Discussion

This method is called before connection(_:didReceive:), allowing the delegate to inspect a protection space before attempting to authenticate against it. By returning true, the delegate indicates that it can handle the form of authentication, which it does in the subsequent call to connection(_:didReceive:). If the delegate returns false, the system attempts to use the user’s keychain to authenticate. If your delegate does not implement this method and the protection space uses client certificate authentication or server trust authentication, the system behaves as if you returned false. The system behaves as if you returned true for all other authentication methods.

Note

This method is not called if the delegate implements the connection(_:willSendRequestFor:) method.

## See Also

### Connection Authentication

func connection(NSURLConnection, willSendRequestFor: URLAuthenticationChallenge)

Tells the delegate that the connection will send a request for an authentication challenge.

func connection(NSURLConnection, didCancel: URLAuthenticationChallenge)

Sent when a connection cancels an authentication challenge.

Deprecated

func connection(NSURLConnection, didReceive: URLAuthenticationChallenge)

Sent when a connection must authenticate a challenge in order to download its request.

Deprecated

func connectionShouldUseCredentialStorage(NSURLConnection) -> Bool

Sent to determine whether the URL loader should use the credential storage for authenticating the connection.

