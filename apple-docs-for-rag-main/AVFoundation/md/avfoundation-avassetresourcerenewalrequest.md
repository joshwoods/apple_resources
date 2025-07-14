

- AVFoundation
-  AVAssetResourceRenewalRequest 

Class

# AVAssetResourceRenewalRequest

An object that encapsulates information about a resource request from a resource loader to renew a previously issued request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetResourceRenewalRequest
```

## Overview

When an AVURLAsset needs to renew a resource, because the renewalDate has been set on a previous loading request, it asks its AVAssetResourceLoader object to assist. The resource loader encapsulates the request information by creating an instance of this object, which it then hands to its delegate for processing. The delegate uses the information in this object to perform the request and report on the success or failure of the operation.

The `AVAssetResourceRenewalRequest` class is a subclass of AVAssetResourceLoadingRequest.

## Relationships

### Inherits From

- AVAssetResourceLoadingRequest

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

class AVAssetResourceLoader

An object that mediates resource requests from a URL asset.

protocol AVAssetResourceLoaderDelegate

Methods you can implement to handle resource-loading requests coming from a URL asset.

class AVAssetResourceLoadingRequest

An object that encapsulates information about a resource request from a resource loader object.

class AVAssetResourceLoadingRequestor

An object that contains information about the originator of a resource-loading request.

class AVAssetResourceLoadingDataRequest

An object for requesting data from a resource that an asset resource-loading request references.

class AVAssetResourceLoadingContentInformationRequest

A query for retrieving essential information about a resource that an asset resource-loading request references.

