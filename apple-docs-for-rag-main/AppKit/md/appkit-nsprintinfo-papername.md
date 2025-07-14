

- AppKit
- NSPrintInfo
-  paperName 

Instance Property

# paperName

The name of the currently selected paper size.

macOS

``` source
var paperName: NSPrinter.PaperName? { get set }
```

## Discussion

The string contains a value such as Letter or Legal. Paper names are implementation specific.

## See Also

### Related Documentation

func dictionary() -> NSMutableDictionary

Returns the print info’s dictionary that contains the printing attributes.

init(dictionary: [NSPrintInfo.AttributeKey : Any])

Returns a printing information object initialized with the parameters in the specified dictionary.

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

struct PaperName

The type you use to specify the name of a type of paper.

var localizedPaperName: String?

The human-readable name of the currently selected paper size, suitable for presentation in user interfaces.

