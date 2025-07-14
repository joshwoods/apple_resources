

- Foundation
- URLProtocolClient
-  urlProtocol(\_:cachedResponseIsValid:) 

Instance Method

# urlProtocol(\_:cachedResponseIsValid:)

Tells the client that a cached response is valid.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urlProtocol(
    _ protocol: URLProtocol,
    cachedResponseIsValid cachedResponse: CachedURLResponse
)
```

**Required**

## Parameters 

`protocol`  

The URL protocol object sending the message.

`cachedResponse`  

The cached response whose validity is being communicated.

