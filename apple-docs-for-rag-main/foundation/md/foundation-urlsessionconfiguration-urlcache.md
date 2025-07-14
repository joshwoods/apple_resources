

- Foundation
- URLSessionConfiguration
-  urlCache 

Instance Property

# urlCache

The URL cache for providing cached responses to requests within the session.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var urlCache: URLCache? { get set }
```

## Mentioned in 

Accessing cached data

## Discussion

This property determines the URL cache object used by tasks within sessions based on this configuration.

To disable caching, set this property to `nil`.

For default sessions, the default value is the shared URL cache object.

For background sessions, the default value is `nil`.

For ephemeral sessions, the default value is a private cache object that stores data in memory only, and is destroyed when you invalidate the session.

## See Also

### Setting caching policies

var requestCachePolicy: NSURLRequest.CachePolicy

A predefined constant that determines when to return a response from the cache.

