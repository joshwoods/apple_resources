

- WebKit
- WebFrameView
-  printDocumentView() Deprecated

Instance Method

# printDocumentView()

Prints the receiver.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func printDocumentView()
```

## Discussion

This method is invoked if the documentViewShouldHandlePrint method returns false.

## See Also

### Printing Views

var canPrintHeadersAndFooters: Bool

A Boolean value indicating whether the receiver can print headers and footers.

Deprecated

func printOperation(with: NSPrintInfo!) -> NSPrintOperation!

Returns a print operation object to print this frame.

Deprecated

var documentViewShouldHandlePrint: Bool

A Boolean value indicating whether the document view should handle a print operation.

Deprecated

