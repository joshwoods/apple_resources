

- WebKit
- WebView
-  isLoading Deprecated

Instance Property

# isLoading

A Boolean that indicates whether the web view is loading content.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var isLoading: Bool { get }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

true if the web view is currently loading any resources; otherwise, false.

## See Also

### Getting and Setting Frame Contents

var selectedFrame: WebFrame!

The frame with the active selection.

Deprecated

var mainFrameURL: String!

The URL that the main frame loads.

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

