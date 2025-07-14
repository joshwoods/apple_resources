

- Foundation
- URLSessionConfiguration
-  requestCachePolicy 

Instance Property

# requestCachePolicy

A predefined constant that determines when to return a response from the cache.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var requestCachePolicy: NSURLRequest.CachePolicy { get set }
```

## Mentioned in 

Accessing cached data

## Discussion

This property determines the request caching policy used by tasks within sessions based on this configuration.

Set this property to one of the constants defined in NSURLRequest.CachePolicy to specify whether the cache policy should depend on expiration dates and age, whether the cache should be disabled entirely, and whether the server should be contacted to determine if the content has changed since it was last requested.

The default value is NSURLRequest.CachePolicy.useProtocolCachePolicy.

## See Also

### Setting caching policies

var urlCache: URLCache?

The URL cache for providing cached responses to requests within the session.

