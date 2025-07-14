

- Foundation
- NSMutableURLRequest
-  cachePolicy 

Instance Property

# cachePolicy

The request’s cache policy.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var cachePolicy: NSURLRequest.CachePolicy { get set }
```

## Discussion

This property is ignored for requests used to construct URLSessionUploadTask and URLSessionDownloadTask objects, as caching is not supported by the URL Loading System for upload or download requests.

## See Also

### Working with a cache policy

enum CachePolicy

The constants used to specify interaction with the cached responses.

