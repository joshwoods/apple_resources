

- AVFoundation
- AVAssetResourceLoadingContentInformationRequest
-  allowedContentTypes 

Instance Property

# allowedContentTypes

The types of data that are accepted as a valid response for the requested resource.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+macOS 10.13.2+tvOS 11.2+visionOS 1.0+

``` source
var allowedContentTypes: [String]? { get }
```

## Discussion

This property contains an array of file format UTIs. When `allowedContentTypes` is non-nil, the value of contentType must be set to a value contained in `allowedContentTypes` or `nil`.

## See Also

### Configuring Content Information

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

