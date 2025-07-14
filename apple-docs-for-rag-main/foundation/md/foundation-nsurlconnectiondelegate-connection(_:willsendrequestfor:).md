

- Foundation
- NSURLConnectionDelegate
-  connection(\_:willSendRequestFor:) 

Instance Method

# connection(\_:willSendRequestFor:)

Tells the delegate that the connection will send a request for an authentication challenge.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func connection(
    _ connection: NSURLConnection,
    willSendRequestFor challenge: URLAuthenticationChallenge
)
```

## Parameters 

`connection`  

The connection sending the message.

`challenge`  

The authentication challenge for which a request is being sent.

## Discussion

This method allows the delegate to make an informed decision about connection authentication at once. If the delegate implements this method, it has no need to implement connection(_:canAuthenticateAgainstProtectionSpace:) or connection(_:didReceive:). In fact, those other methods are not invoked (except on older operating systems, where applicable).

In this method,you *must* invoke one of the challenge-responder methods (URLAuthenticationChallengeSender protocol):

- use(_:for:)

- continueWithoutCredential(for:)

- cancel(_:)

- performDefaultHandling(for:)

- rejectProtectionSpaceAndContinue(with:)

Important

Your delegate method is called on the thread where the connection is scheduled. Always call the methods above on that same thread.

You might also want to analyze `challenge` for the authentication scheme and the proposed credential before calling a URLAuthenticationChallengeSender method. You should never assume that a proposed credential is present. You can either create your own credential and respond with that, or you can send the proposed credential back. (Because this object is immutable, if you want to change it you must copy it and then modify the copy.)

## See Also

### Related Documentation

URL Loading System

Interact with URLs and communicate with servers using standard Internet protocols.

### Connection Authentication

func connection(NSURLConnection, canAuthenticateAgainstProtectionSpace: URLProtectionSpace) -> Bool

Sent to determine whether the delegate is able to respond to a protection space’s form of authentication.

Deprecated

func connection(NSURLConnection, didCancel: URLAuthenticationChallenge)

Sent when a connection cancels an authentication challenge.

Deprecated

func connection(NSURLConnection, didReceive: URLAuthenticationChallenge)

Sent when a connection must authenticate a challenge in order to download its request.

Deprecated

func connectionShouldUseCredentialStorage(NSURLConnection) -> Bool

Sent to determine whether the URL loader should use the credential storage for authenticating the connection.

