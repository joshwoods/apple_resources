

- Foundation
- URLProtocolClient
-  urlProtocol(\_:didCancel:) 

Instance Method

# urlProtocol(\_:didCancel:)

Tells the client that an authentication challenge has been canceled.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urlProtocol(
    _ protocol: URLProtocol,
    didCancel challenge: URLAuthenticationChallenge
)
```

**Required**

## Parameters 

`protocol`  

The URL protocol object sending the message.

`challenge`  

The authentication challenge that was canceled.

## See Also

### Handling authentication challenges

func urlProtocol(URLProtocol, didReceive: URLAuthenticationChallenge)

Tells the client that the URL Loading System received an authentication challenge.

**Required**

