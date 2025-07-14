

- WebKit
- WebPreferences
-  cacheModel Deprecated

Instance Property

# cacheModel

The cache model for the web views associated with the receiver.

macOS 10.3–10.14Deprecated

``` source
var cacheModel: WebCacheModel { get set }
```

## Discussion

Possible values are described in WebCacheModel.

Set this property to optimize WebKit’s cache footprint (on disk and in memory) to best fit the use of the web view. If a web view is used only for a single webpage, use the WebCacheModel.documentViewer constant instead.

## See Also

### Caching

var usesPageCache: Bool

A Boolean that indicates whether the web views associated with the receiver should use the shared page cache.

Deprecated

