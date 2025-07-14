

- WebKit
- WebBackForwardList
-  pageCacheSize() Deprecated

Instance Method

# pageCacheSize()

Returns the maximum number of pages that the receiver can cache.

macOS

``` source
func pageCacheSize() -> Int
```

Deprecated

Use the usesPageCache method in WebPreferences instead.

## Return Value

The maximum number of pages that can be cached.

## See Also

### Page Caching

func setPageCacheSize(Int)

Sets the maximum number of pages the receiver can cache.

Deprecated

