

- AVFoundation
- AVAssetResourceLoadingRequest
-  isCancelled 

Instance Property

# isCancelled

A Boolean value that indicates whether the request has been cancelled.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var isCancelled: Bool { get }
```

## Discussion

true when the resource loader cancels the loading of a request, just prior to sending the message resourceLoader(_:didCancel:) to the delegate.

## See Also

### Reporting the Result of the Request

var response: URLResponse?

The URL response for the loading request.

func finishLoading()

Causes the receiver to treat the processing of the request as complete.

func finishLoading(with: (any Error)?)

Causes the receiver to handle the failure to load a resource for which a resource loader’s delegate took responsibility.

var isFinished: Bool

A Boolean value that indicates whether loading of the resource has finished.

func finishLoading(with: URLResponse?, data: Data?, redirect: URLRequest?)

Causes the receiver to finish loading a resource for which a resource loader’s delegate took responsibility .

Deprecated

