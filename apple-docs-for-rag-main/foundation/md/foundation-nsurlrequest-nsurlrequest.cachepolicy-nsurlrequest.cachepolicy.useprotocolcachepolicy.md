

- Foundation
- NSURLRequest
- NSURLRequest.CachePolicy
-  NSURLRequest.CachePolicy.useProtocolCachePolicy 

Case

# NSURLRequest.CachePolicy.useProtocolCachePolicy

Use the caching logic defined in the protocol implementation, if any, for a particular URL load request.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case useProtocolCachePolicy
```

## Mentioned in 

Accessing cached data

## Discussion

This is the default policy for URL load requests.

### HTTP caching behavior

For the HTTP and HTTPS protocols, NSURLRequest.CachePolicy.useProtocolCachePolicy performs the following behavior:

1.  If a cached response does not exist for the request, the URL loading system fetches the data from the originating source.

2.  Otherwise, if the cached response does not indicate that it must be revalidated every time, and if the cached response is not stale (past its expiration date), the URL loading system returns the cached response.

3.  If the cached response is stale or requires revalidation, the URL loading system makes a HEAD request to the originating source to see if the resource has changed. If so, the URL loading system fetches the data from the originating source. Otherwise, it returns the cached response.

This behavior is illustrated in the figure below.

Note

For the formal definition of these semantics, see RFC 2616.

Important

If you are making HTTP or HTTPS byte-range requests, always use the NSURLRequest.CachePolicy.reloadIgnoringLocalCacheData policy instead.

## See Also

### Policies

case reloadIgnoringLocalCacheData

The URL load should be loaded only from the originating source.

case reloadIgnoringLocalAndRemoteCacheData

Ignore local cache data, and instruct proxies and other intermediates to disregard their caches so far as the protocol allows.

static var reloadIgnoringCacheData: NSURLRequest.CachePolicy

Replaced by NSURLRequest.CachePolicy.reloadIgnoringLocalCacheData.

case returnCacheDataElseLoad

Use existing cache data, regardless or age or expiration date, loading from originating source only if there is no cached data.

case returnCacheDataDontLoad

Use existing cache data, regardless or age or expiration date, and fail if no cached data is available.

case reloadRevalidatingCacheData

Use cache data if the origin source can validate it; otherwise, load from the origin.

case reloadIgnoringLocalCacheData

The URL load should be loaded only from the originating source.

case reloadIgnoringLocalAndRemoteCacheData

Ignore local cache data, and instruct proxies and other intermediates to disregard their caches so far as the protocol allows.

static var reloadIgnoringCacheData: NSURLRequest.CachePolicy

Replaced by NSURLRequest.CachePolicy.reloadIgnoringLocalCacheData.

case returnCacheDataElseLoad

Use existing cache data, regardless or age or expiration date, loading from originating source only if there is no cached data.

case returnCacheDataDontLoad

Use existing cache data, regardless or age or expiration date, and fail if no cached data is available.

case reloadRevalidatingCacheData

Use cache data if the origin source can validate it; otherwise, load from the origin.

