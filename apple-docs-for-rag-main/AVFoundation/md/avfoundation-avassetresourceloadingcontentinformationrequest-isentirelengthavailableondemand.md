

- AVFoundation
- AVAssetResourceLoadingContentInformationRequest
-  isEntireLengthAvailableOnDemand 

Instance Property

# isEntireLengthAvailableOnDemand

A Boolean value that indicates whether asset data loading can expect data immediately.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var isEntireLengthAvailableOnDemand: Bool { get set }
```

## Discussion

Before you finish loading an AVAssetResourceLoadingRequest, if its contentInformationRequest isn’t `nil`, set the value to true to indicate that all asset data is available. This may be true because the data is fully cached, or because the custom URL scheme ultimately refers to files on local storage, which allows for significant data flow optimizations.

For backward compatibility, this property defaults to false.

## See Also

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

