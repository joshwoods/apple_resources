

- Foundation
- NSURLRequest
- NSURLRequest.CachePolicy
-  NSURLRequest.CachePolicy.returnCacheDataDontLoad 

Case

# NSURLRequest.CachePolicy.returnCacheDataDontLoad

Use existing cache data, regardless or age or expiration date, and fail if no cached data is available.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case returnCacheDataDontLoad
```

## Mentioned in 

Accessing cached data

## Discussion

If there is no existing data in the cache corresponding to a URL load request, no attempt is made to load the data from the originating source, and the load is considered to have failed. This constant specifies a behavior that is similar to an “offline” mode.

## See Also

### Policies

case useProtocolCachePolicy

Use the caching logic defined in the protocol implementation, if any, for a particular URL load request.

case reloadIgnoringLocalCacheData

The URL load should be loaded only from the originating source.

case reloadIgnoringLocalAndRemoteCacheData

Ignore local cache data, and instruct proxies and other intermediates to disregard their caches so far as the protocol allows.

static var reloadIgnoringCacheData: NSURLRequest.CachePolicy

Replaced by NSURLRequest.CachePolicy.reloadIgnoringLocalCacheData.

case returnCacheDataElseLoad

Use existing cache data, regardless or age or expiration date, loading from originating source only if there is no cached data.

case reloadRevalidatingCacheData

Use cache data if the origin source can validate it; otherwise, load from the origin.

case useProtocolCachePolicy

Use the caching logic defined in the protocol implementation, if any, for a particular URL load request.

case reloadIgnoringLocalCacheData

The URL load should be loaded only from the originating source.

case reloadIgnoringLocalAndRemoteCacheData

Ignore local cache data, and instruct proxies and other intermediates to disregard their caches so far as the protocol allows.

static var reloadIgnoringCacheData: NSURLRequest.CachePolicy

Replaced by NSURLRequest.CachePolicy.reloadIgnoringLocalCacheData.

case returnCacheDataElseLoad

Use existing cache data, regardless or age or expiration date, loading from originating source only if there is no cached data.

case reloadRevalidatingCacheData

Use cache data if the origin source can validate it; otherwise, load from the origin.

