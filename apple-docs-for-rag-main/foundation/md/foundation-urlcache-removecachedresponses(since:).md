

- Foundation
- URLCache
-  removeCachedResponses(since:) 

Instance Method

# removeCachedResponses(since:)

Clears the given cache of any cached responses since the provided date.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeCachedResponses(since date: Date)
```

## Parameters 

`date`  

The earliest date of responses that should remain in the cache. Any responses with dates later than this parameter should be removed.

## Mentioned in 

Accessing cached data

## See Also

### Removing cached objects

func removeCachedResponse(for: URLRequest)

Removes the cached URL response for a specified URL request.

func removeCachedResponse(for: URLSessionDataTask)

Removes the cached URL response for a specified data task.

func removeAllCachedResponses()

Clears the receiver’s cache, removing all stored cached URL responses.

