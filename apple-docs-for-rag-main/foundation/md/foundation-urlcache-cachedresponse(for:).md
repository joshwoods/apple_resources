

- Foundation
- URLCache
-  cachedResponse(for:) 

Instance Method

# cachedResponse(for:)

Returns the cached URL response in the cache for the specified URL request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func cachedResponse(for request: URLRequest) -> CachedURLResponse?
```

## Parameters 

`request`  

The URL request whose cached response is desired.

## Return Value

The cached URL response for `request`, or `nil` if no response has been cached.

## Mentioned in 

Accessing cached data

## Discussion

If you override this method, you should also override getCachedResponse(for:completionHandler:).

## See Also

### Getting and storing cached objects

func storeCachedResponse(CachedURLResponse, for: URLRequest)

Stores a cached URL response for a specified request.

func getCachedResponse(for: URLSessionDataTask, completionHandler: (CachedURLResponse?) -> Void)

Gets the cached URL response for a data task, passing it to the provided completion handler.

func storeCachedResponse(CachedURLResponse, for: URLSessionDataTask)

Stores a cached URL response for a specified data task.

