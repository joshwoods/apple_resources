

- Foundation
- NSURLRequest
-  init(url:cachePolicy:timeoutInterval:) 

Initializer

# init(url:cachePolicy:timeoutInterval:)

Creates a URL request with the specified URL, cache policy, and timeout values.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    url URL: URL,
    cachePolicy: NSURLRequest.CachePolicy,
    timeoutInterval: TimeInterval
)
```

## Parameters 

`URL`  

The URL for the request.

`cachePolicy`  

The cache policy for the request.

`timeoutInterval`  

The timeout interval for the request, in seconds.

## Return Value

The initialized URL request.

## Discussion

This is the designated initializer for `NSURLRequest`.

## See Also

### Creating requests

convenience init(url: URL)

Creates a URL request for a specified URL.

