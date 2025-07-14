

- WebKit
- WebView
-  shouldCloseWithWindow Deprecated

Instance Property

# shouldCloseWithWindow

A Boolean that indicates whether the web view should close when its window or host window closes.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var shouldCloseWithWindow: Bool { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

If true, the web view should close; otherwise, it should not.

## See Also

### Closing the View

func close()

Closes the web view when it’s no longer needed.

Deprecated

