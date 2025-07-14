

- UIKit
- UIPrintInteractionController
-  printingItem 

Instance Property

# printingItem

A single ready-to-print object.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var printingItem: Any? { get set }
```

## Discussion

The object must be an instance of the NSURL, NSData, or UIImage class. An object of the first two types must reference or contain image data or PDF data. `NSURL` objects must use the `file:` or any scheme that can return an NSData object with a registered protocol. Image data (including that encapsulated by UIImage) must be in a format supported by the Image I/O framework; see UIImage for more information. The object is released at the end of the print job. The default value is `nil`.

If you set this property, `UIPrintInteractionController` sets the printingItems, printPageRenderer, and printFormatter properties to `nil`. (You can only set one of these properties for a print job).

If this property is set and the showsPageRange property is set to true—and the printing item is a PDF document of more than one page—the printing options include the control for selecting a page range.

## See Also

### Providing the source of printable content

var printingItems: [Any]?

An array of ready-to-print objects.

var printPageRenderer: UIPrintPageRenderer?

An object that draws pages of printable content when UIKit requests it.

var printFormatter: UIPrintFormatter?

An object that lays out the content of pages according to the kind of content.

