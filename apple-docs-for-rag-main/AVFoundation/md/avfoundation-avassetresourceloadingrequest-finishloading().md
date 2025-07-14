

- AVFoundation
- AVAssetResourceLoadingRequest
-  finishLoading() 

Instance Method

# finishLoading()

Causes the receiver to treat the processing of the request as complete.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func finishLoading()
```

## Discussion

If a dataRequest is present and the resource does not contain the full extent of the data that has been requested according to the values of the requestedOffset and requestedLength properties of the request, invoke `finishLoading` after providing as much of the requested data as the resource contains.

## See Also

### Reporting the Result of the Request

var response: URLResponse?

The URL response for the loading request.

var isCancelled: Bool

A Boolean value that indicates whether the request has been cancelled.

func finishLoading(with: (any Error)?)

Causes the receiver to handle the failure to load a resource for which a resource loader’s delegate took responsibility.

var isFinished: Bool

A Boolean value that indicates whether loading of the resource has finished.

func finishLoading(with: URLResponse?, data: Data?, redirect: URLRequest?)

Causes the receiver to finish loading a resource for which a resource loader’s delegate took responsibility .

Deprecated

