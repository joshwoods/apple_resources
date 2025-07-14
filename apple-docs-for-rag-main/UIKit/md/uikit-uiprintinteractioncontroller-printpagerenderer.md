

- UIKit
- UIPrintInteractionController
-  printPageRenderer 

Instance Property

# printPageRenderer

An object that draws pages of printable content when UIKit requests it.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var printPageRenderer: UIPrintPageRenderer? { get set }
```

## Discussion

The object assigned to this property must be an instance of a custom subclass of UIPrintPageRenderer. The `UIPrintInteractionController` class retains the page-renderer object and releases it at the end of the print job. The default value is `nil`.

If you set this property, `UIPrintInteractionController` sets the printingItems, printingItem, printFormatter properties to `nil`. (Only one of these properties can be set for a print job.)

If this property is set and the showsPageRange property is set to true—and the rendered content is greater than one page—the printing options include the control for selecting a page range.

## See Also

### Providing the source of printable content

var printingItem: Any?

A single ready-to-print object.

var printingItems: [Any]?

An array of ready-to-print objects.

var printFormatter: UIPrintFormatter?

An object that lays out the content of pages according to the kind of content.

