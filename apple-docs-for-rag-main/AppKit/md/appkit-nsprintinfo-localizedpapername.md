

- AppKit
- NSPrintInfo
-  localizedPaperName 

Instance Property

# localizedPaperName

The human-readable name of the currently selected paper size, suitable for presentation in user interfaces.

macOS

``` source
var localizedPaperName: String? { get }
```

## Discussion

This is typically different from the value of paperName, which is almost never suitable for presentation to the user.

## See Also

### Managing the Printing Rectangle

var paperSize: NSSize

The size of the paper.

var topMargin: CGFloat

The top margin to the specified size.

var bottomMargin: CGFloat

The height of the bottom margin.

var leftMargin: CGFloat

The width of the left margin.

var rightMargin: CGFloat

The width of the right margin.

var imageablePageBounds: NSRect

The imageable area of a sheet of paper specified by the print info.

var orientation: NSPrintInfo.PaperOrientation

The orientation attribute.

enum PaperOrientation

Constants that describe the orientation of printing on a page.

var paperName: NSPrinter.PaperName?

The name of the currently selected paper size.

struct PaperName

The type you use to specify the name of a type of paper.

