

- Foundation
- URLCache
-  storeCachedResponse(\_:for:) 

Instance Method

# storeCachedResponse(\_:for:)

Stores a cached URL response for a specified request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func storeCachedResponse(
    _ cachedResponse: CachedURLResponse,
    for request: URLRequest
)
```

## Parameters 

`cachedResponse`  

The cached URL response to store.

`request`  

The request for which the cached URL response is being stored.

## Mentioned in 

Accessing cached data

## Discussion

If you override this method, you should also override storeCachedResponse(_:for:).

## See Also

### Getting and storing cached objects

func cachedResponse(for: URLRequest) -> CachedURLResponse?

Returns the cached URL response in the cache for the specified URL request.

func getCachedResponse(for: URLSessionDataTask, completionHandler: (CachedURLResponse?) -> Void)

Gets the cached URL response for a data task, passing it to the provided completion handler.

func storeCachedResponse(CachedURLResponse, for: URLSessionDataTask)

Stores a cached URL response for a specified data task.

