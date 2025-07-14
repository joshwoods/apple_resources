

- AVFoundation
-  AVAssetResourceLoader 

Class

# AVAssetResourceLoader

An object that mediates resource requests from a URL asset.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetResourceLoader
```

## Overview

You do not create resource loader objects yourself. Instead, you retrieve a resource loader from the resourceLoader property of an AVURLAsset object and use it to assign your custom delegate object.

The delegate you associate with this object must adopt the AVAssetResourceLoaderDelegate protocol. For more information, see AVAssetResourceLoaderDelegate.

## Topics

### Accessing the Delegate

func setDelegate((any AVAssetResourceLoaderDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue to use with the resource loader.

var delegate: (any AVAssetResourceLoaderDelegate)?

The delegate object to use when handling resource requests.

protocol AVAssetResourceLoaderDelegate

Methods you can implement to handle resource-loading requests coming from a URL asset.

var delegateQueue: dispatch_queue_t?

The dispatch queue to use when handling resource requests.

### Loading Content Keys

var preloadsEligibleContentKeys: Bool

A Boolean value that indicates whether content keys will be loaded as quickly as possible.

### Supporting Common Media Client Data

var sendsCommonMediaClientDataAsHTTPHeaders: Bool

A Boolean value that indicates whether to enable attaching Common Media Client Data as HTTP request headers.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Resource loading

protocol AVAssetResourceLoaderDelegate

Methods you can implement to handle resource-loading requests coming from a URL asset.

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

