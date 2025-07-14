

- AVFoundation
- AVAssetResourceLoadingRequest
-  response 

Instance Property

# response

The URL response for the loading request.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
@NSCopying
var response: URLResponse? { get set }
```

## Discussion

The value of this property is an instance of URLResponse, indicating a response to the loading request. If no response is needed, the value of this property is `nil`.

## See Also

### Reporting the Result of the Request

func finishLoading()

Causes the receiver to treat the processing of the request as complete.

var isCancelled: Bool

A Boolean value that indicates whether the request has been cancelled.

func finishLoading(with: (any Error)?)

Causes the receiver to handle the failure to load a resource for which a resource loader’s delegate took responsibility.

var isFinished: Bool

A Boolean value that indicates whether loading of the resource has finished.

func finishLoading(with: URLResponse?, data: Data?, redirect: URLRequest?)

Causes the receiver to finish loading a resource for which a resource loader’s delegate took responsibility .

Deprecated

