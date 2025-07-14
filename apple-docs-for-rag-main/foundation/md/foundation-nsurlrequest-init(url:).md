

- Foundation
- NSURLRequest
-  init(url:) 

Initializer

# init(url:)

Creates a URL request for a specified URL.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(url URL: URL)
```

## Parameters 

`URL`  

The URL for the request.

## Return Value

The initialized URL request.

## Discussion

The request is created with the with the default cache policy (NSURLRequest.CachePolicy.useProtocolCachePolicy), and the default timeout interval (60 seconds).

## See Also

### Creating requests

init(url: URL, cachePolicy: NSURLRequest.CachePolicy, timeoutInterval: TimeInterval)

Creates a URL request with the specified URL, cache policy, and timeout values.

