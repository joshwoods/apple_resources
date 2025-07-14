

- Foundation
- CachedURLResponse
-  userInfo 

Instance Property

# userInfo

The cached response’s user info dictionary.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var userInfo: [AnyHashable : Any]? { get }
```

## Mentioned in 

Accessing cached data

## Discussion

This value is `nil` if there is no user info dictionary.

## See Also

### Getting cached URL response properties

var data: Data

The cached response’s data.

var response: URLResponse

The URL response object associated with the instance.

var storagePolicy: URLCache.StoragePolicy

The cached response’s storage policy.

