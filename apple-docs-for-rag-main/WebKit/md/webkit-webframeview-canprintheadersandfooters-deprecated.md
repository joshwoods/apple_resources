

- WebKit
- WebFrameView
-  canPrintHeadersAndFooters Deprecated

Instance Property

# canPrintHeadersAndFooters

A Boolean value indicating whether the receiver can print headers and footers.

macOS 10.3–10.14Deprecated

``` source
@MainActor
var canPrintHeadersAndFooters: Bool { get }
```

## Discussion

true if the receiver can print headers and footers; otherwise, false.

## See Also

### Printing Views

func printOperation(with: NSPrintInfo!) -> NSPrintOperation!

Returns a print operation object to print this frame.

Deprecated

var documentViewShouldHandlePrint: Bool

A Boolean value indicating whether the document view should handle a print operation.

Deprecated

func printDocumentView()

Prints the receiver.

Deprecated

