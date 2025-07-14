

- Foundation
- URLProtocolClient
-  urlProtocol(\_:wasRedirectedTo:redirectResponse:) 

Instance Method

# urlProtocol(\_:wasRedirectedTo:redirectResponse:)

Tells the client that the protocol implementation has been redirected.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urlProtocol(
    _ protocol: URLProtocol,
    wasRedirectedTo request: URLRequest,
    redirectResponse: URLResponse
)
```

**Required**

## Parameters 

`protocol`  

The URL protocol object sending the message.

`request`  

The new request that the original request was redirected to.

`redirectResponse`  

The response from the original request that caused the redirect.

