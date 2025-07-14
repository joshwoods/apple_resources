

- AVFoundation
-  AVAssetResourceLoadingContentInformationRequest 

Class

# AVAssetResourceLoadingContentInformationRequest

A query for retrieving essential information about a resource that an asset resource-loading request references.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetResourceLoadingContentInformationRequest
```

## Overview

When a resource loading delegate, which must implement the AVAssetResourceLoaderDelegate protocol, receives an instance of AVAssetResourceLoadingRequest when the resourceLoader(_:shouldWaitForLoadingOfRequestedResource:) is invoked and accepts responsibility for loading the resource, it must check whether the contentInformationRequest property of the AVAssetResourceLoadingRequest is not `nil`. Whenever the value is not `nil`, the request includes a query for the information that `AVAssetResourceLoadingContentInformationRequest` encapsulates. In response to such queries, the resource loading delegate should set the values of the content information request’s properties appropriately before invoking the AVAssetResourceLoadingRequest method finishLoading().

When finishLoading() is invoked, the values of the properties of its contentInformationRequest property will, in part, determine how the requested resource is processed. For example, if the requested resource’s URL is the URL of an AVURLAsset and contentType is set by the resource loading delegate to a value that the underlying media system doesn’t recognize as a supported media file type, operations on the `AVURLAsset`, such as playback, are likely to fail.

## Topics

### Configuring Content Information

var allowedContentTypes: [String]?

The types of data that are accepted as a valid response for the requested resource.

var contentType: String?

The UTI that specifies the type of data contained by the requested resource.

var contentLength: Int64

The length, in bytes, of the requested resource.

var isByteRangeAccessSupported: Bool

A Boolean value that indicates whether random access to arbitrary ranges of bytes of the resource is supported.

var renewalDate: Date?

The date at which a new resource loading request will be issued for resources that expire, if the media system still requires it.

var isEntireLengthAvailableOnDemand: Bool

A Boolean value that indicates whether asset data loading can expect data immediately.

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

class AVAssetResourceLoader

An object that mediates resource requests from a URL asset.

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

