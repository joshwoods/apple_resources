

- AVFoundation
- AVAssetResourceLoaderDelegate
-  resourceLoader(\_:shouldWaitForLoadingOfRequestedResource:) 

Instance Method

# resourceLoader(\_:shouldWaitForLoadingOfRequestedResource:)

Asks the delegate if it wants to load the requested resource.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
optional func resourceLoader(
    _ resourceLoader: AVAssetResourceLoader,
    shouldWaitForLoadingOfRequestedResource loadingRequest: AVAssetResourceLoadingRequest
) -> Bool
```

## Parameters 

`resourceLoader`  

The resource loader object that is making the request.

`loadingRequest`  

The loading request object that contains information about the requested resource.

## Return Value

true if your delegate can load the resource specified by the `loadingRequest` parameter or false if it cannot.

## Discussion

The resource loader object calls this method when assistance is required of your code to load the specified resource. For example, the resource loader might call this method to load decryption keys that have been specified using a custom URL scheme.

Returning true from this method, implies only that the receiver will load, or at least attempt to load, the resource. In some implementations, the actual work of loading the resource might be initiated on another thread, running asynchronously to the resource loading delegate; whether the work begins immediately or merely soon is an implementation detail of the client application.

You can load the resource synchronously or asynchronously. In both cases, you must indicate success or failure of the operation by calling the finishLoading(with:data:redirect:) or finishLoading(with:) method of the request object when you finish. If you load the resource asynchronously, you must also store a strong reference to the object in the `loadingRequest` parameter before returning from this method.

If you return false from this method, the resource loader treats the loading of the resource as having failed.

## See Also

### Processing Resource Requests

func resourceLoader(AVAssetResourceLoader, shouldWaitForRenewalOfRequestedResource: AVAssetResourceRenewalRequest) -> Bool

Tells the delegate when assistance is required of the application to renew a resource.

func resourceLoader(AVAssetResourceLoader, didCancel: AVAssetResourceLoadingRequest)

Informs the delegate that a prior loading request has been cancelled.

