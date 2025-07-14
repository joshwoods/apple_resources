

- Foundation
- URLSessionDelegate
-  urlSession(\_:didReceive:completionHandler:) 

Instance Method

# urlSession(\_:didReceive:completionHandler:)

Requests credentials from the delegate in response to a session-level authentication request from the remote server.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
optional func urlSession(
    _ session: URLSession,
    didReceive challenge: URLAuthenticationChallenge,
    completionHandler: @escaping (URLSession.AuthChallengeDisposition, URLCredential?) -> Void
)
```

``` source
optional func urlSession(
    _ session: URLSession,
    didReceive challenge: URLAuthenticationChallenge
) async -> (URLSession.AuthChallengeDisposition, URLCredential?)
```

## Parameters 

`session`  

The session containing the task that requested authentication.

`challenge`  

An object that contains the request for authentication.

`completionHandler`  

A handler that your delegate method must call. This completion handler takes the following parameters::

- `disposition`—One of several constants that describes how the challenge should be handled.

- `credential`—The credential that should be used for authentication if disposition is `NSURLSessionAuthChallengeUseCredential`, otherwise `NULL`.

## Mentioned in 

Performing manual server trust authentication

## Discussion

This method is called in two situations:

- When a remote server asks for client certificates or Windows NT LAN Manager (NTLM) authentication, to allow your app to provide appropriate credentials

- When a session first establishes a connection to a remote server that uses SSL or TLS, to allow your app to verify the server’s certificate chain

If you do not implement this method, the session calls its delegate’s urlSession(_:task:didReceive:completionHandler:) method instead.

Note

This method handles *only* the NSURLAuthenticationMethodNTLM, NSURLAuthenticationMethodNegotiate, NSURLAuthenticationMethodClientCertificate, and NSURLAuthenticationMethodServerTrust authentication types. For all other authentication schemes, the session calls *only* the urlSession(_:task:didReceive:completionHandler:) method.

## See Also

### Handling authentication challenges

enum AuthChallengeDisposition

Constants passed by session or task delegates to the provided continuation block in response to an authentication challenge.

