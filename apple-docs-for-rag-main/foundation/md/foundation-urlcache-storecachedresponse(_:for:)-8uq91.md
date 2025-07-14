

- Foundation
- URLCache
-  storeCachedResponse(\_:for:) 

Instance Method

# storeCachedResponse(\_:for:)

Stores a cached URL response for a specified data task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func storeCachedResponse(
    _ cachedResponse: CachedURLResponse,
    for dataTask: URLSessionDataTask
)
```

## Parameters 

`cachedResponse`  

The cached URL response to store for this data task.

`dataTask`  

The data task whose response is to be cached.

## See Also

### Getting and storing cached objects

func cachedResponse(for: URLRequest) -> CachedURLResponse?

Returns the cached URL response in the cache for the specified URL request.

func storeCachedResponse(CachedURLResponse, for: URLRequest)

Stores a cached URL response for a specified request.

func getCachedResponse(for: URLSessionDataTask, completionHandler: (CachedURLResponse?) -> Void)

Gets the cached URL response for a data task, passing it to the provided completion handler.

