

- Foundation
- URLProtocolClient
-  urlProtocol(\_:didReceive:) 

Instance Method

# urlProtocol(\_:didReceive:)

Tells the client that the URL Loading System received an authentication challenge.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urlProtocol(
    _ protocol: URLProtocol,
    didReceive challenge: URLAuthenticationChallenge
)
```

**Required**

## Parameters 

`protocol`  

The URL protocol object sending the message.

`challenge`  

The authentication challenge that has been received.

## Discussion

The protocol client guarantees that it will answer the request on the same thread that called this method. The client may add a default credential to the challenge it issues to the connection delegate, if `protocol` did not provide one.

## See Also

### Handling authentication challenges

func urlProtocol(URLProtocol, didCancel: URLAuthenticationChallenge)

Tells the client that an authentication challenge has been canceled.

**Required**

