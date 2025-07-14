

- Foundation
- URLRequest
-  init(url:cachePolicy:timeoutInterval:) 

Initializer

# init(url:cachePolicy:timeoutInterval:)

Creates and initializes a URL request with the given URL, cache policy, and timeout interval.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    url: URL,
    cachePolicy: URLRequest.CachePolicy = .useProtocolCachePolicy,
    timeoutInterval: TimeInterval = 60.0
)
```

## Parameters 

`url`  

The URL for the request.

`cachePolicy`  

The cache policy for the request. The default is NSURLRequest.CachePolicy.useProtocolCachePolicy.

`timeoutInterval`  

The timeout interval for the request. The default is `60.0`. See the commentary for the timeoutInterval for more information on timeout intervals.

