

- WebKit
- WebFrameView
-  documentView Deprecated

Instance Property

# documentView

The subview that displays the web content.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var documentView: (any NSView & WebDocumentView)! { get }
```

## Discussion

Use allowsScrolling to enable scrolling of this view.

