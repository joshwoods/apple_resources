

- AppKit
- NSView
-  locationOfPrintRect(\_:) 

Instance Method

# locationOfPrintRect(\_:)

Invoked by printView(_:) to determine the location of the region of the view being printed on the physical page.

macOS

``` source
@MainActor
func locationOfPrintRect(_ rect: NSRect) -> NSPoint
```

## Parameters 

`rect`  

A rectangle defining a region of the view; it is expressed in the default coordinate system of the page.

## Return Value

A point to be used for setting the origin for `aRect`, whose size the view can examine in order to properly place it. It is expressed in the default coordinate system of the page.

## Discussion

The default implementation places `aRect` according to the status of the NSPrintInfo object for the print job. By default it places the image in the upper-left corner of the page, but if the `NSPrintInfo` methods isHorizontallyCentered or isVerticallyCentered return true, it centers a single-page image along the appropriate axis. A multiple-page document, however, is always placed so the divided pieces can be assembled at their edges.

## See Also

### Handling Pagination

var heightAdjustLimit: CGFloat

The fraction of the page that can be pushed onto the next page during automatic pagination to prevent items such as lines of text from being divided across pages.

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

