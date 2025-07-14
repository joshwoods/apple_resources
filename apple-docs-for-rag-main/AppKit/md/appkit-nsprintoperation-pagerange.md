

- AppKit
- NSPrintOperation
-  pageRange 

Instance Property

# pageRange

The range of pages associated with the print operation.

macOS 10.5+

``` source
@MainActor
var pageRange: NSRange { get }
```

## Return Value

The range of page numbers. Page numbers are one-based values where the index of page one is 1, the index of page two is 2, and so on. Depending on the information returned by the printing view, the starting page number may not be 1. Also, if the number of pages being printed is not known, the page count may be set to `NSIntegerMax`.

## See Also

### Related Documentation

func knowsPageRange(NSRangePointer) -> Bool

Returns true if the view handles page boundaries, false otherwise.

### Managing Page Information

var currentPage: Int

The current page number being printed.

var pageOrder: NSPrintOperation.PageOrder

The print order for the pages of the operation.

enum PageOrder

Constants that specify the page order.

