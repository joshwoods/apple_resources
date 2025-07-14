

- AppKit
- NSPrintInfo
-  imageablePageBounds 

Instance Property

# imageablePageBounds

The imageable area of a sheet of paper specified by the print info.

macOS

``` source
var imageablePageBounds: NSRect { get }
```

## Discussion

This property takes into account the current printer, paper size, and orientation settings, but not scaling factors. “Imageable area” is the maximum area that can possibly be marked on by the printer hardware, not the area defined by the current margin settings.

The origin (0, 0) of the rectangle is in the lower-left corner of the oriented sheet. The imageable bounds may extend past the edges of the sheet when, for example, a printer driver specifies it so that borderless printing can be done reliably.

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

var orientation: NSPrintInfo.PaperOrientation

The orientation attribute.

enum PaperOrientation

Constants that describe the orientation of printing on a page.

var paperName: NSPrinter.PaperName?

The name of the currently selected paper size.

struct PaperName

The type you use to specify the name of a type of paper.

var localizedPaperName: String?

The human-readable name of the currently selected paper size, suitable for presentation in user interfaces.

