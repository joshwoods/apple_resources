

- UIKit
- UIPrintPageRenderer
-  addPrintFormatter(\_:startingAtPageAt:) 

Instance Method

# addPrintFormatter(\_:startingAtPageAt:)

Adds a print formatter to the page renderer starting at the specified page.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func addPrintFormatter(
    _ formatter: UIPrintFormatter,
    startingAtPageAt pageIndex: Int
)
```

## Parameters 

`formatter`  

The UIPrintFormatter object to add to the page renderer. A print formatter can be an instance of UISimpleTextPrintFormatter, UIMarkupTextPrintFormatter, or UIViewPrintFormatter.

`pageIndex`  

The index identifying the first page with which the print formatter should be associated with. This value overrides the startPage property of the print formatter.

## Discussion

You can dissociate a print formatter from its page renderer by calling the removeFromPrintPageRenderer() method on the print formatter.

## See Also

### Managing print formatters

func printFormattersForPage(at: Int) -> [UIPrintFormatter]?

Returns the print formatters for a specified page.

var printFormatters: [UIPrintFormatter]?

The print formatters for the page renderer.

