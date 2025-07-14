

- Foundation
- CachedURLResponse
-  init(response:data:) 

Initializer

# init(response:data:)

Creates a cached URL response instance.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    response: URLResponse,
    data: Data
)
```

## Parameters 

`response`  

The response to cache.

`data`  

The data to cache.

## Return Value

A cached URL response object, containing the response and data.

## Discussion

The cache storage policy is set to the default, URLCache.StoragePolicy.allowed, and the user info dictionary is set to `nil`.

## See Also

### Creating a cached URL response

init(response: URLResponse, data: Data, userInfo: [AnyHashable : Any]?, storagePolicy: URLCache.StoragePolicy)

Creates a cached URL response with a given server response, data, user-info dictionary, and storage policy.

