

- AVFoundation
-  AVURLAssetHTTPCookiesKey 

Global Variable

# AVURLAssetHTTPCookiesKey

The HTTP cookies that a URL asset may send with HTTP requests.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.15+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
let AVURLAssetHTTPCookiesKey: String
```

## Discussion

By default, AVURLAsset only has access to cookies in the client’s default cookie storage that apply to the asset’s URL. You can supplement the cookies available to the asset by setting this initialization option.

Cookies don’t apply to non-HTTP(S) URLs. In HTTP Live Streaming, the system may issue many HTTP requests (for example, media, crypt key, variant index) to different paths or hosts. In these cases, HTTP requests won’t contain any cookies that don’t apply to the AVURLAsset URL.

## See Also

### Options

let AVURLAssetAllowsCellularAccessKey: String

A Boolean value that indicates whether the system can make network requests on behalf of the asset when connected to a cellular network.

let AVURLAssetAllowsConstrainedNetworkAccessKey: String

A Boolean value that indicates whether the system allows network requests on behalf of this asset to use the constrained interface.

let AVURLAssetAllowsExpensiveNetworkAccessKey: String

A Boolean value that indicates whether the system allows network requests on behalf of this asset to use the expensive interface.

let AVURLAssetHTTPUserAgentKey: String

A key that specifies the user agent of requests that an asset makes.

let AVURLAssetOverrideMIMETypeKey: String

A key that specifies the MIME type to use to identify the format of a media resource.

let AVURLAssetPreferPreciseDurationAndTimingKey: String

A Boolean value that indicates whether the asset should provide accurate duration and precise random access by time.

let AVURLAssetPrimarySessionIdentifierKey: String

Specifies a UUID to set as the session identifier for HTTP requests that the asset makes.

let AVURLAssetReferenceRestrictionsKey: String

A value that represents the restrictions used by the asset when resolving references to external media data.

let AVURLAssetShouldSupportAliasDataReferencesKey: String

A Boolean value that indicates whether the system parses and resolves alias data references in the asset.

let AVURLAssetURLRequestAttributionKey: String

A value that specifies the attribution of the URLs that this asset requests.

