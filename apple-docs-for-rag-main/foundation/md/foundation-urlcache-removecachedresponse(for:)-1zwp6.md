

- Foundation
- URLCache
-  removeCachedResponse(for:) 

Instance Method

# removeCachedResponse(for:)

Removes the cached URL response for a specified data task.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeCachedResponse(for dataTask: URLSessionDataTask)
```

## Parameters 

`dataTask`  

A task whose URL request’s corresponding cached URL response should be removed. If there is no corresponding cached URL response, no action is taken.

## See Also

### Removing cached objects

func removeCachedResponse(for: URLRequest)

Removes the cached URL response for a specified URL request.

func removeCachedResponses(since: Date)

Clears the given cache of any cached responses since the provided date.

func removeAllCachedResponses()

Clears the receiver’s cache, removing all stored cached URL responses.

