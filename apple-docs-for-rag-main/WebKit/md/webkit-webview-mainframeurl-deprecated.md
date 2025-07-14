

- WebKit
- WebView
-  mainFrameURL Deprecated

Instance Property

# mainFrameURL

The URL that the main frame loads.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var mainFrameURL: String! { get set }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

Functionally equivalent to invoking `[[webView mainFrame] loadRequest:[NSURLRequest requestWithURL: [NSURL URLWithString:URLString]]]`.

## See Also

### Getting and Setting Frame Contents

var isLoading: Bool

A Boolean that indicates whether the web view is loading content.

Deprecated

var selectedFrame: WebFrame!

The frame with the active selection.

Deprecated

var mainFrameTitle: String!

The HTML title of the loaded page.

Deprecated

var mainFrameIcon: NSImage!

The site’s favicon.

Deprecated

var mainFrameDocument: DOMDocument!

The DOM document for the main frame.

Deprecated

