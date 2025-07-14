

- Foundation
- NSURLConnectionDelegate
-  connectionShouldUseCredentialStorage(\_:) 

Instance Method

# connectionShouldUseCredentialStorage(\_:)

Sent to determine whether the URL loader should use the credential storage for authenticating the connection.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func connectionShouldUseCredentialStorage(_ connection: NSURLConnection) -> Bool
```

## Parameters 

`connection`  

The connection sending the message.

## Discussion

This method is called before any attempt to authenticate is made.

If you return false, the connection does not consult the credential storage automatically, and does not store credentials. However, in your connection:didReceiveAuthenticationChallenge: method, you can consult the credential storage yourself and store credentials yourself, as needed.

Not implementing this method is the same as returning true.

Important

Prior to iOS 7 and OS X v10.9, the `connectionShouldUseCredentialStorage:` method is never called on delegates that implement the connection(_:willSendRequestFor:) method.

In later operating systems, if the delegate implements the connection(_:willSendRequestFor:) method, the `connectionShouldUseCredentialStorage:` method is called *only* if the app’s deployment target is at least iOS 7 or OS X v10.9.

## See Also

### Connection Authentication

func connection(NSURLConnection, willSendRequestFor: URLAuthenticationChallenge)

Tells the delegate that the connection will send a request for an authentication challenge.

func connection(NSURLConnection, canAuthenticateAgainstProtectionSpace: URLProtectionSpace) -> Bool

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

Deprecated

func connection(NSURLConnection, didCancel: URLAuthenticationChallenge)

Sent when a connection cancels an authentication challenge.

Deprecated

func connection(NSURLConnection, didReceive: URLAuthenticationChallenge)

Sent when a connection must authenticate a challenge in order to download its request.

Deprecated

