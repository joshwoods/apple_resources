

- UIKit
- UIPrintPageRenderer
-  printFormattersForPage(at:) 

Instance Method

# printFormattersForPage(at:)

Returns the print formatters for a specified page.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func printFormattersForPage(at pageIndex: Int) -> [UIPrintFormatter]?
```

## Parameters 

`pageIndex`  

The index of a page of printable content.

## Return Value

An array of UIPrintFormatter objects. A print formatter can be an instance of UISimpleTextPrintFormatter, UIMarkupTextPrintFormatter, or UIViewPrintFormatter.

## Discussion

A print formatter is associated with a starting page of printable content through the addPrintFormatter(_:startingAtPageAt:) method or the startPage property of UIPrintFormatter. The number of pages from that page is determined by the pageCount property, which UIPrintFormatter computes based on layout metrics and content.

## See Also

### Managing print formatters

func addPrintFormatter(UIPrintFormatter, startingAtPageAt: Int)

Adds a print formatter to the page renderer starting at the specified page.

var printFormatters: [UIPrintFormatter]?

The print formatters for the page renderer.

