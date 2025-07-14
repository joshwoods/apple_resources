

- WebKit
- WebView
-  mainFrameTitle Deprecated

Instance Property

# mainFrameTitle

The HTML title of the loaded page.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var mainFrameTitle: String! { get }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

The HTML title of the loaded page. Returns `@""` if the loaded document is not HTML.

## See Also

### Getting and Setting Frame Contents

var isLoading: Bool

A Boolean that indicates whether the web view is loading content.

Deprecated

var selectedFrame: WebFrame!

The frame with the active selection.

Deprecated

var mainFrameURL: String!

The URL that the main frame loads.

Deprecated

var mainFrameIcon: NSImage!

The site’s favicon.

Deprecated

var mainFrameDocument: DOMDocument!

The DOM document for the main frame.

Deprecated

