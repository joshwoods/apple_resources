

- AVFoundation
-  AVAssetResourceLoaderDelegate 

Protocol

# AVAssetResourceLoaderDelegate

Methods you can implement to handle resource-loading requests coming from a URL asset.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
protocol AVAssetResourceLoaderDelegate : NSObjectProtocol
```

## Overview

A class should adopt this protocol when associated with the asset’s resource loader—that is, an instance of the AVAssetResourceLoader class. The resource loader works with your delegate to process the request.

## Topics

### Processing Resource Requests

func resourceLoader(AVAssetResourceLoader, shouldWaitForLoadingOfRequestedResource: AVAssetResourceLoadingRequest) -> Bool

Asks the delegate if it wants to load the requested resource.

func resourceLoader(AVAssetResourceLoader, shouldWaitForRenewalOfRequestedResource: AVAssetResourceRenewalRequest) -> Bool

Tells the delegate when assistance is required of the application to renew a resource.

func resourceLoader(AVAssetResourceLoader, didCancel: AVAssetResourceLoadingRequest)

Informs the delegate that a prior loading request has been cancelled.

### Processing Authentication Challenges

func resourceLoader(AVAssetResourceLoader, shouldWaitForResponseTo: URLAuthenticationChallenge) -> Bool

Tells the delegate that assistance is required of the application to respond to an authentication challenge.

func resourceLoader(AVAssetResourceLoader, didCancel: URLAuthenticationChallenge)

Informs the delegate that a prior authentication challenge has been cancelled.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Resource loading

class AVAssetResourceLoader

An object that mediates resource requests from a URL asset.

class AVAssetResourceLoadingRequest

An object that encapsulates information about a resource request from a resource loader object.

class AVAssetResourceRenewalRequest

An object that encapsulates information about a resource request from a resource loader to renew a previously issued request.

class AVAssetResourceLoadingRequestor

An object that contains information about the originator of a resource-loading request.

class AVAssetResourceLoadingDataRequest

An object for requesting data from a resource that an asset resource-loading request references.

class AVAssetResourceLoadingContentInformationRequest

A query for retrieving essential information about a resource that an asset resource-loading request references.

