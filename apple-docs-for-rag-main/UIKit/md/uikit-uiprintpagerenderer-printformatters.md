

- UIKit
- UIPrintPageRenderer
-  printFormatters 

Instance Property

# printFormatters

The print formatters for the page renderer.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var printFormatters: [UIPrintFormatter]? { get set }
```

## Discussion

The elements of the array are UIPrintFormatter objects. A print formatter can be an instance of UISimpleTextPrintFormatter, UIMarkupTextPrintFormatter, or UIViewPrintFormatter. Print formatters added this way to a page renderer are associated with page ranges through each print formatter’s startPage and pageCount properties.

## See Also

### Managing print formatters

func addPrintFormatter(UIPrintFormatter, startingAtPageAt: Int)

Adds a print formatter to the page renderer starting at the specified page.

func printFormattersForPage(at: Int) -> [UIPrintFormatter]?

Returns the print formatters for a specified page.

