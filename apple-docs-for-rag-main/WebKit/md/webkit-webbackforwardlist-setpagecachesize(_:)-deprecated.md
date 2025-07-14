

- WebKit
- WebBackForwardList
-  setPageCacheSize(\_:) Deprecated

Instance Method

# setPageCacheSize(\_:)

Sets the maximum number of pages the receiver can cache.

macOS

``` source
func setPageCacheSize(_ size: Int)
```

Deprecated

Use the usesPageCache method in WebPreferences instead.

## Parameters 

`size`  

The maximum number of pages that can be cached.

## Discussion

The default page cache size can vary depending on the computer’s configuration. Use pageCacheSize() to get the current setting.

## See Also

### Page Caching

func pageCacheSize() -> Int

Returns the maximum number of pages that the receiver can cache.

Deprecated

