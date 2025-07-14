

- WebKit
- WebView
-  selectedFrame Deprecated

Instance Property

# selectedFrame

The frame with the active selection.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var selectedFrame: WebFrame! { get }
```

Deprecated

No longer supported; please adopt WKWebView.

## Discussion

If it doesn’t exist, the frame that contains a non-zero-length selection; otherwise, `nil`.

## See Also

### Getting and Setting Frame Contents

var isLoading: Bool

A Boolean that indicates whether the web view is loading content.

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

