

- UIKit
- UIPrintFormatter
-  startPage 

Instance Property

# startPage

The index of the first page that the print formatter lays out.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var startPage: Int { get set }
```

## Discussion

The value is a zero-based index. You can set the starting page of a print formatter by assigning an index to this property or by passing one as the second argument of the addPrintFormatter(_:startingAtPageAt:) method of UIPrintPageRenderer.

## See Also

### Managing pagination

var pageCount: Int

The number of pages to print.

