

- Foundation
- URLCache
-  removeCachedResponse(for:) 

Instance Method

# removeCachedResponse(for:)

Removes the cached URL response for a specified URL request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeCachedResponse(for request: URLRequest)
```

## Parameters 

`request`  

The URL request whose cached URL response should be removed. If there is no corresponding cached URL response, no action is taken.

## Mentioned in 

Accessing cached data

## Discussion

If you override this method, you should also override removeCachedResponse(for:).

## See Also

### Removing cached objects

func removeCachedResponse(for: URLSessionDataTask)

Removes the cached URL response for a specified data task.

func removeCachedResponses(since: Date)

Clears the given cache of any cached responses since the provided date.

func removeAllCachedResponses()

Clears the receiver’s cache, removing all stored cached URL responses.

