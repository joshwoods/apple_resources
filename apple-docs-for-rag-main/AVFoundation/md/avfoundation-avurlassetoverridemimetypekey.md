

- AVFoundation
-  AVURLAssetOverrideMIMETypeKey 

Global Variable

# AVURLAssetOverrideMIMETypeKey

A key that specifies the MIME type to use to identify the format of a media resource.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
let AVURLAssetOverrideMIMETypeKey: String
```

## Discussion

If you specify a value for this key, the system uses it to determine how to handle or parse the media resource, and ignores any other information that may be available, such as the URL path extension or a server-provided MIME type.

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

