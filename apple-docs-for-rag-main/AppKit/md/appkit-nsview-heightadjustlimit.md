

- AppKit
- NSView
-  heightAdjustLimit 

Instance Property

# heightAdjustLimit

The fraction of the page that can be pushed onto the next page during automatic pagination to prevent items such as lines of text from being divided across pages.

macOS

``` source
@MainActor
var heightAdjustLimit: CGFloat { get }
```

## Discussion

The value of this property is a floating point number in the range `0.0` to `1.0`. This fraction is used to calculate the bottom edge limit for an adjustPageHeightNew(_:top:bottom:limit:) message.

## See Also

### Handling Pagination

var widthAdjustLimit: CGFloat

The fraction of the page that can be pushed onto the next page during automatic pagination to prevent items such as small images or text columns from being divided across pages.

func adjustPageWidthNew(UnsafeMutablePointer&lt;CGFloat>, left: CGFloat, right: CGFloat, limit: CGFloat)

Overridden by subclasses to adjust page width during automatic pagination.

func adjustPageHeightNew(UnsafeMutablePointer&lt;CGFloat>, top: CGFloat, bottom: CGFloat, limit: CGFloat)

Overridden by subclasses to adjust page height during automatic pagination.

func knowsPageRange(NSRangePointer) -> Bool

Returns true if the view handles page boundaries, false otherwise.

func rectForPage(Int) -> NSRect

Implemented by subclasses to determine the portion of the view to be printed for the specified page number.

func locationOfPrintRect(NSRect) -> NSPoint

Invoked by printView(_:) to determine the location of the region of the view being printed on the physical page.

