

- AVFoundation
- AVAssetResourceLoaderDelegate
-  resourceLoader(\_:didCancel:) 

Instance Method

# resourceLoader(\_:didCancel:)

Informs the delegate that a prior loading request has been cancelled.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
optional func resourceLoader(
    _ resourceLoader: AVAssetResourceLoader,
    didCancel loadingRequest: AVAssetResourceLoadingRequest
)
```

## Parameters 

`resourceLoader`  

The resource loader.

`loadingRequest`  

The loading request that has been cancelled.

## Discussion

Previously issued loading requests can be cancelled when data from the resource is no longer required or when a loading request is superseded by new requests for data from the same resource.

For example, if to complete a seek operation it becomes necessary to load a range of bytes that’s different from a range previously requested, the prior request may be cancelled while the delegate is still handling it.

## See Also

### Processing Resource Requests

func resourceLoader(AVAssetResourceLoader, shouldWaitForLoadingOfRequestedResource: AVAssetResourceLoadingRequest) -> Bool

Asks the delegate if it wants to load the requested resource.

func resourceLoader(AVAssetResourceLoader, shouldWaitForRenewalOfRequestedResource: AVAssetResourceRenewalRequest) -> Bool

Tells the delegate when assistance is required of the application to renew a resource.

