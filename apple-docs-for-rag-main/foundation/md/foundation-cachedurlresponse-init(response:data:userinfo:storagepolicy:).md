

- Foundation
- CachedURLResponse
-  init(response:data:userInfo:storagePolicy:) 

Initializer

# init(response:data:userInfo:storagePolicy:)

Creates a cached URL response with a given server response, data, user-info dictionary, and storage policy.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    response: URLResponse,
    data: Data,
    userInfo: [AnyHashable : Any]? = nil,
    storagePolicy: URLCache.StoragePolicy
)
```

## Parameters 

`response`  

The response to cache.

`data`  

The data to cache.

`userInfo`  

An optional dictionary of user information. May be `nil`.

`storagePolicy`  

The storage policy for the cached response.

## Return Value

A cached URL response object, containing the response and data.

## See Also

### Creating a cached URL response

init(response: URLResponse, data: Data)

Creates a cached URL response instance.

