

- AVFoundation
- AVAssetResourceLoadingRequest
-  isFinished 

Instance Property

# isFinished

A Boolean value that indicates whether loading of the resource has finished.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var isFinished: Bool { get }
```

## Discussion

The value of this property is false initially. The value changes to true when the delegate object handling the request calls the finishLoading(with:data:redirect:) or finishLoading(with:) method.

## See Also

### Reporting the Result of the Request

var response: URLResponse?

The URL response for the loading request.

func finishLoading()

Causes the receiver to treat the processing of the request as complete.

var isCancelled: Bool

A Boolean value that indicates whether the request has been cancelled.

func finishLoading(with: (any Error)?)

Causes the receiver to handle the failure to load a resource for which a resource loader’s delegate took responsibility.

func finishLoading(with: URLResponse?, data: Data?, redirect: URLRequest?)

Causes the receiver to finish loading a resource for which a resource loader’s delegate took responsibility .

Deprecated

