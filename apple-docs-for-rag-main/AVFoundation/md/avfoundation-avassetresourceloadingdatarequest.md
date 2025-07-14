

- AVFoundation
-  AVAssetResourceLoadingDataRequest 

Class

# AVAssetResourceLoadingDataRequest

An object for requesting data from a resource that an asset resource-loading request references.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
class AVAssetResourceLoadingDataRequest
```

## Overview

The AVAssetResourceLoaderDelegate uses the `AVAssetResourceLoadingDataRequest` class to do the actual data reading, and its methods will be invoked, as necessary, to acquire data for the AVAssetResourceLoadingRequest instance.

When the resource loading delegate, which implements the AVAssetResourceLoaderDelegate protocol, receives an instance of AVAssetResourceLoadingRequest as the second parameter of the delegate’s resourceLoader(_:shouldWaitForLoadingOfRequestedResource:) method, it has the option of accepting responsibility for loading the referenced resource. If it accepts that responsibility, by returning true, it must check whether the dataRequest property of the AVAssetResourceLoadingRequest instance is not `nil`. If it is not `nil`, the resource loading delegate is informed of the range of bytes within the resource that are required by the underlying media system. In response, the data is provided by one or more invocations of respond(with:) as required to provide the requested data. The data can be provided in increments determined by the resource loading delegate according to convenience or efficiency.

When the AVAssetResourceLoadingRequest method finishLoading() is invoked, the data request is considered fully satisfied. If the entire range of bytes requested has not yet been provided, the underlying media system assumes that the resource’s length is limited to the provided content.

## Topics

### Providing Data to a Request

func respond(with: Data)

Provides data to the loading request.

var requestedLength: Int

The length, in bytes, of the data requested.

var requestedOffset: Int64

The position within the resource of the first byte requested.

var currentOffset: Int64

The position within the resource of the next byte.

var requestsAllDataToEndOfResource: Bool

A Boolean value that indicates the entire remaining length of the resource from the offest to the end of the resource is being requested.

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

class AVAssetResourceLoadingContentInformationRequest

A query for retrieving essential information about a resource that an asset resource-loading request references.

