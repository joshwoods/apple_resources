

- Foundation
- NSURLConnectionDelegate
-  connection(\_:didCancel:) Deprecated

Instance Method

# connection(\_:didCancel:)

Sent when a connection cancels an authentication challenge.

iOS 2.0–8.0DeprecatediPadOS 2.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.2–10.10DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
optional func connection(
    _ connection: NSURLConnection,
    didCancel challenge: URLAuthenticationChallenge
)
```

Deprecated

Use -connection:willSendRequestForAuthenticationChallenge: instead.

## Parameters 

`connection`  

The connection sending the message.

`challenge`  

The challenge that was canceled.

## See Also

### Connection Authentication

func connection(NSURLConnection, willSendRequestFor: URLAuthenticationChallenge)

Tells the delegate that the connection will send a request for an authentication challenge.

func connection(NSURLConnection, canAuthenticateAgainstProtectionSpace: URLProtectionSpace) -> Bool

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

Deprecated

func connection(NSURLConnection, didReceive: URLAuthenticationChallenge)

Sent when a connection must authenticate a challenge in order to download its request.

Deprecated

func connectionShouldUseCredentialStorage(NSURLConnection) -> Bool

Sent to determine whether the URL loader should use the credential storage for authenticating the connection.

