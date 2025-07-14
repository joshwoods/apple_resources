

- WebKit
- WebView
-  drawsBackground Deprecated

Instance Property

# drawsBackground

A Boolean that indicates whether the web view draws a background.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var drawsBackground: Bool { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

If true, a default background is drawn; if false, it is not.

## See Also

### Drawing

var shouldUpdateWhileOffscreen: Bool

A Boolean that inidicates whether the web view should update even when it is not in a window that is currently visible.

Deprecated

