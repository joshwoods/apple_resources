

- AVFoundation
-  AVAssetResourceLoadingRequestor 

Class

# AVAssetResourceLoadingRequestor

An object that contains information about the originator of a resource-loading request.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
class AVAssetResourceLoadingRequestor
```

## Topics

### Retrieving Expired Session Reports

var providesExpiredSessionReports: Bool

A Boolean value that indicates whether the requestor provides expired session reports.

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

class AVAssetResourceLoadingDataRequest

An object for requesting data from a resource that an asset resource-loading request references.

class AVAssetResourceLoadingContentInformationRequest

A query for retrieving essential information about a resource that an asset resource-loading request references.

