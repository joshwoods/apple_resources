

- AVFoundation
-  AVAssetResourceLoadingRequest 

Class

# AVAssetResourceLoadingRequest

An object that encapsulates information about a resource request from a resource loader object.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetResourceLoadingRequest
```

## Overview

When an AVURLAsset object needs help loading a resource, it asks its AVAssetResourceLoader object to assist. The resource loader encapsulates the request information by creating an instance of this object, which it then hands to its delegate object for processing. The delegate uses the information in this object to perform the request and report on the success or failure of the operation.

## Topics

### Accessing the Request Data

var request: URLRequest

The URL request object for the resource.

var requestor: AVAssetResourceLoadingRequestor

The asset resource requestor that made the request.

var contentInformationRequest: AVAssetResourceLoadingContentInformationRequest?

The information for a requested resource.

var dataRequest: AVAssetResourceLoadingDataRequest?

The range of requested resource data.

var redirect: URLRequest?

An URL request instance if the loading request was redirected.

func streamingContentKeyRequestData(forApp: Data, contentIdentifier: Data, options: [String : Any]?) throws -> Data

Obtains key request data for a specific combination of application and content.

Deprecated

func persistentContentKey(fromKeyVendorResponse: Data, options: [String : Any]?) throws -> Data

Obtains a persistable content key from a context.

Deprecated

let AVAssetResourceLoadingRequestStreamingContentKeyRequestRequiresPersistentKey: String

Specifies whether the content key request requires a persistable key to be returned from the key vendor.

Deprecated

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

func finishLoading(with: URLResponse?, data: Data?, redirect: URLRequest?)

Causes the receiver to finish loading a resource for which a resource loader’s delegate took responsibility .

Deprecated

## Relationships

### Inherits From

- NSObject

### Inherited By

- AVAssetResourceRenewalRequest

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

class AVAssetResourceRenewalRequest

An object that encapsulates information about a resource request from a resource loader to renew a previously issued request.

class AVAssetResourceLoadingRequestor

An object that contains information about the originator of a resource-loading request.

class AVAssetResourceLoadingDataRequest

An object for requesting data from a resource that an asset resource-loading request references.

class AVAssetResourceLoadingContentInformationRequest

A query for retrieving essential information about a resource that an asset resource-loading request references.

