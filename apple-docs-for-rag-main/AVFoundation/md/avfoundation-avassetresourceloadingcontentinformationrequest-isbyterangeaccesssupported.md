

- AVFoundation
- AVAssetResourceLoadingContentInformationRequest
-  isByteRangeAccessSupported 

Instance Property

# isByteRangeAccessSupported

A Boolean value that indicates whether random access to arbitrary ranges of bytes of the resource is supported.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var isByteRangeAccessSupported: Bool { get set }
```

## Discussion

Before finishing loading an AVAssetResourceLoadingRequest instance, if its contentInformationRequest property is not `nil`, set the value of this property to true if it supports random access to arbitrary ranges of bytes of the resource.

If this property is not true for resources that must be loaded incrementally, loading of the resource may fail. Such resources include anything that contains media data.

If byte range access is supported portions of the resource can be requested more than once.

## See Also

### Configuring Content Information

var allowedContentTypes: [String]?

The types of data that are accepted as a valid response for the requested resource.

var contentType: String?

The UTI that specifies the type of data contained by the requested resource.

var contentLength: Int64

The length, in bytes, of the requested resource.

var renewalDate: Date?

The date at which a new resource loading request will be issued for resources that expire, if the media system still requires it.

var isEntireLengthAvailableOnDemand: Bool

A Boolean value that indicates whether asset data loading can expect data immediately.

