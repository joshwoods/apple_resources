

- AVFoundation
-  AVURLAssetAllowsCellularAccessKey 

Global Variable

# AVURLAssetAllowsCellularAccessKey

A Boolean value that indicates whether the system can make network requests on behalf of the asset when connected to a cellular network.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.15+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
let AVURLAssetAllowsCellularAccessKey: String
```

## Discussion

The default behavior of AVURLAsset allows requests over cellular networks. Set this value to false at initialization time to restrict the default behavior.

## See Also

### Options

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

