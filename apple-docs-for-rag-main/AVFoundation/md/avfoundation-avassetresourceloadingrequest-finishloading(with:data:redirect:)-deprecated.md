

- AVFoundation
- AVAssetResourceLoadingRequest
-  finishLoading(with:data:redirect:) Deprecated

Instance Method

# finishLoading(with:data:redirect:)

Causes the receiver to finish loading a resource for which a resource loader’s delegate took responsibility .

macOS 10.15–10.15DeprecatedtvOS 9.0–9.0Deprecated

``` source
func finishLoading(
    with response: URLResponse?,
    data: Data?,
    redirect: URLRequest?
)
```

Deprecated

This method is deprecated. Use the following methods and properties instead: the response property to provide the response object, the redirect property when redirecting a request, invoking the dataRequest instance’srespond(with:) method to provide data, and the finishLoading() method to indicate that loading is finished.

## Parameters 

`response`  

The response object for the requested resource. Use the request object in the receiver’s request property to get information about the requested resource.

`data`  

The data of the resource. If no data is available, specify `nil`.

`redirect`  

When redirecting a resource request, use this parameter to specify the corresponding NSURLRequest object. If you are handling the request and not redirecting it, specify `nil`.

## Discussion

When a resource loader’s delegate takes responsibility for loading a resource, it calls this method to indicate that the resource was loaded successfully. This method marks the loading request as finished and returns the provided data back to the resource loader object for processing.

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

var isFinished: Bool

A Boolean value that indicates whether loading of the resource has finished.

