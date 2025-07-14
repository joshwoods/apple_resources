

- WebKit
- WebFrameView
-  printOperation(with:) Deprecated

Instance Method

# printOperation(with:)

Returns a print operation object to print this frame.

macOS 10.3–10.14Deprecated

``` source
@MainActor
func printOperation(with printInfo: NSPrintInfo!) -> NSPrintOperation!
```

## Parameters 

`printInfo`  

Information about the print settings needed to print this frame. See NSPrintInfo for more information about this object.

## Return Value

An `NSPrintOperation` object set up to print this frame. See NSPrintOperation for more information about this object.

## See Also

### Printing Views

var canPrintHeadersAndFooters: Bool

A Boolean value indicating whether the receiver can print headers and footers.

Deprecated

var documentViewShouldHandlePrint: Bool

A Boolean value indicating whether the document view should handle a print operation.

Deprecated

func printDocumentView()

Prints the receiver.

Deprecated

