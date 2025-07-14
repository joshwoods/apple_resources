

- AVFoundation
- AVAssetResourceLoaderDelegate
-  resourceLoader(\_:shouldWaitForRenewalOfRequestedResource:) 

Instance Method

# resourceLoader(\_:shouldWaitForRenewalOfRequestedResource:)

Tells the delegate when assistance is required of the application to renew a resource.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
optional func resourceLoader(
    _ resourceLoader: AVAssetResourceLoader,
    shouldWaitForRenewalOfRequestedResource renewalRequest: AVAssetResourceRenewalRequest
) -> Bool
```

## Parameters 

`resourceLoader`  

The resource loader.

`renewalRequest`  

An instance of `AVAssetResourceRenewalRequest` that provides information about the requested resource.

## Return Value

true if the delegate can renew the resource; otherwise false.

## Discussion

Delegates receive this message when assistance is required to renew a resource previously loaded by resourceLoader(_:shouldWaitForLoadingOfRequestedResource:). For example, this method is invoked to for decryption keys that require renewal, as indicated in a response to a prior invocation of resourceLoader(_:shouldWaitForLoadingOfRequestedResource:).

If the result is true, the resource loader expects invocation, either subsequently or immediately, of either the `AVAssetResourceRenewalRequest` method `finishLoading` or `finishLoadingWithError:`. If you intend to finish loading the resource after your handling of this message returns, you must retain the `renewalRequest` until after loading is finished.

If the result is false, the resource loader treats the loading of the resource as having failed.

Note

If the delegate’s implementation of -resourceLoader(_:shouldWaitForLoadingOfRequestedResource:) returns true without finishing the loading request immediately, it may be invoked again with another loading request before the prior request is finished; therefore in such cases the delegate should be prepared to manage multiple loading requests.

## See Also

### Processing Resource Requests

func resourceLoader(AVAssetResourceLoader, shouldWaitForLoadingOfRequestedResource: AVAssetResourceLoadingRequest) -> Bool

Asks the delegate if it wants to load the requested resource.

func resourceLoader(AVAssetResourceLoader, didCancel: AVAssetResourceLoadingRequest)

Informs the delegate that a prior loading request has been cancelled.

