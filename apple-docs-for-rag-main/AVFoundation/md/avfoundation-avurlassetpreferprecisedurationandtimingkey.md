

- AVFoundation
-  AVURLAssetPreferPreciseDurationAndTimingKey 

Global Variable

# AVURLAssetPreferPreciseDurationAndTimingKey

A Boolean value that indicates whether the asset should provide accurate duration and precise random access by time.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
let AVURLAssetPreferPreciseDurationAndTimingKey: String
```

## Discussion

Setting a value of true indicates longer loading times are acceptable in cases where you require precise timing. Container formats like QuickTime and MPEG-4 provide sufficient timing information and don’t require additional parsing to retrieve it. Other formats don’t provide sufficient summary information, and the system can’t accurately calculate the resource’s duration and timing without examining the media content.

If you only intend to play the asset, the default value of false is sufficient because AVPlayer supports approximate random access by time when full precision isn’t available. If you intend to insert the asset into AVMutableComposition or AVMutableMovie, precise random access is typically desirable, and you should set this option to true.

## See Also

### Options

let AVURLAssetAllowsCellularAccessKey: String

A Boolean value that indicates whether the system can make network requests on behalf of the asset when connected to a cellular network.

let AVURLAssetAllowsConstrainedNetworkAccessKey: String

A Boolean value that indicates whether the system allows network requests on behalf of this asset to use the constrained interface.

let AVURLAssetAllowsExpensiveNetworkAccessKey: String

A Boolean value that indicates whether the system allows network requests on behalf of this asset to use the expensive interface.

let AVURLAssetHTTPCookiesKey: String

The HTTP cookies that a URL asset may send with HTTP requests.

let AVURLAssetHTTPUserAgentKey: String

A key that specifies the user agent of requests that an asset makes.

let AVURLAssetOverrideMIMETypeKey: String

A key that specifies the MIME type to use to identify the format of a media resource.

let AVURLAssetPrimarySessionIdentifierKey: String

Specifies a UUID to set as the session identifier for HTTP requests that the asset makes.

let AVURLAssetReferenceRestrictionsKey: String

A value that represents the restrictions used by the asset when resolving references to external media data.

let AVURLAssetShouldSupportAliasDataReferencesKey: String

A Boolean value that indicates whether the system parses and resolves alias data references in the asset.

let AVURLAssetURLRequestAttributionKey: String

A value that specifies the attribution of the URLs that this asset requests.

