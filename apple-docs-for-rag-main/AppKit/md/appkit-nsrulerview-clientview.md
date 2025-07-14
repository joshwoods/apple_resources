

- AppKit
- NSRulerView
-  clientView 

Instance Property

# clientView

The receiver’s client view, if it has one.

macOS

``` source
@MainActor
weak var clientView: NSView? { get set }
```

## Discussion

`aView` is either the document view of the NSScrollView that contains the receiver or a subview of the document view.

