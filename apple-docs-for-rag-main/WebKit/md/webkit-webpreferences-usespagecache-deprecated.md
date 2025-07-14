

- WebKit
- WebPreferences
-  usesPageCache Deprecated

Instance Property

# usesPageCache

A Boolean that indicates whether the web views associated with the receiver should use the shared page cache.

macOS 10.3–10.14Deprecated

``` source
var usesPageCache: Bool { get set }
```

## Discussion

true if the web views should use a page cache; otherwise, false.

Pages are cached when they are added to a back-forward list, and removed from the cache when they are removed from a back-forward list. Because the page cache is global, caching a page in one back-forward list may cause a page in another back-forward list to be removed from the cache.

## See Also

### Caching

var cacheModel: WebCacheModel

The cache model for the web views associated with the receiver.

Deprecated

