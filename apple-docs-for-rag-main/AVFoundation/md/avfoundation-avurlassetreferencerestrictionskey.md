

- AVFoundation
-  AVURLAssetReferenceRestrictionsKey 

Global Variable

# AVURLAssetReferenceRestrictionsKey

A value that represents the restrictions used by the asset when resolving references to external media data.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
let AVURLAssetReferenceRestrictionsKey: String
```

## Discussion

The corresponding value is an NSNumber that wraps an AVAssetReferenceRestrictions enum value, or the logical combination of multiple enum values, that indicate the restrictions the asset uses when resolving references to external media data.

Some assets can contain references to media data stored outside the asset’s container file, for example in another file. Use this key to specify the policy to use when the asset encounters these references. If an asset contains one or more references to a type forbidden by the reference restriction, loading of asset properties fails, and you can’t use this asset with other AVFoundation objects, such as AVPlayerItem or AVAssetExportSession.

## Topics

### Data Types

struct AVAssetReferenceRestrictions

Restrictions to use when resolving references to external media data.

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

let AVURLAssetPreferPreciseDurationAndTimingKey: String

A Boolean value that indicates whether the asset should provide accurate duration and precise random access by time.

let AVURLAssetPrimarySessionIdentifierKey: String

Specifies a UUID to set as the session identifier for HTTP requests that the asset makes.

let AVURLAssetShouldSupportAliasDataReferencesKey: String

A Boolean value that indicates whether the system parses and resolves alias data references in the asset.

let AVURLAssetURLRequestAttributionKey: String

A value that specifies the attribution of the URLs that this asset requests.

