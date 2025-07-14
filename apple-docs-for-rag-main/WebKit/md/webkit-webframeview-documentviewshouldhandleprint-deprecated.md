

- WebKit
- WebFrameView
-  documentViewShouldHandlePrint Deprecated

Instance Property

# documentViewShouldHandlePrint

A Boolean value indicating whether the document view should handle a print operation.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var documentViewShouldHandlePrint: Bool { get }
```

## Discussion

If this method returns false, the application terminates its print operation and sends printDocumentView() to the web frame view.

## See Also

### Printing Views

var canPrintHeadersAndFooters: Bool

A Boolean value indicating whether the receiver can print headers and footers.

Deprecated

func printOperation(with: NSPrintInfo!) -> NSPrintOperation!

Returns a print operation object to print this frame.

Deprecated

func printDocumentView()

Prints the receiver.

Deprecated

