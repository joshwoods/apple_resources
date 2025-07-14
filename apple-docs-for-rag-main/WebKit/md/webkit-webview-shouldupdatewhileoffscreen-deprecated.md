

- WebKit
- WebView
-  shouldUpdateWhileOffscreen Deprecated

Instance Property

# shouldUpdateWhileOffscreen

A Boolean that inidicates whether the web view should update even when it is not in a window that is currently visible.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var shouldUpdateWhileOffscreen: Bool { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

If true, the web view updates regardless if it is visible. If false, it updates only if it is visible, possibly improving performance, and then updates automatically when it becomes visible. The default value is true.

## See Also

### Drawing

var drawsBackground: Bool

A Boolean that indicates whether the web view draws a background.

Deprecated

