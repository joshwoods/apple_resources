

- UIKit
- UIPrintInteractionController
-  printFormatter 

Instance Property

# printFormatter

An object that lays out the content of pages according to the kind of content.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var printFormatter: UIPrintFormatter? { get set }
```

## Discussion

Assign to this property an instance of one of the concrete subclasses of UIPrintFormatter: UISimpleTextPrintFormatter, UIMarkupTextPrintFormatter, and UIViewPrintFormatter. This object is released at the end of the print job.

If you set this property, `UIPrintInteractionController` sets the printingItems, printingItem, and printPageRenderer properties to `nil`. (Only one of these properties can be set for a print job.)

If this property is set and the showsPageRange property is set to true—and if the formatter represents content of more than one page—the printing options include the control for selecting a page range.

## See Also

### Providing the source of printable content

var printingItem: Any?

A single ready-to-print object.

var printingItems: [Any]?

An array of ready-to-print objects.

var printPageRenderer: UIPrintPageRenderer?

An object that draws pages of printable content when UIKit requests it.

