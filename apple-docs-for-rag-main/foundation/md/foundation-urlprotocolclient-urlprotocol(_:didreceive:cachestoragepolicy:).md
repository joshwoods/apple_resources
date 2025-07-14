

- Foundation
- URLProtocolClient
-  urlProtocol(\_:didReceive:cacheStoragePolicy:) 

Instance Method

# urlProtocol(\_:didReceive:cacheStoragePolicy:)

Tells the client that the protocol implementation has created a response object for the request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func urlProtocol(
    _ protocol: URLProtocol,
    didReceive response: URLResponse,
    cacheStoragePolicy policy: URLCache.StoragePolicy
)
```

**Required**

## Parameters 

`protocol`  

The URL protocol object sending the message.

`response`  

The newly available response object.

`policy`  

The cache storage policy for the response.

## Discussion

The implementation should use the provided cache storage policy to determine whether to store the response in a cache.

