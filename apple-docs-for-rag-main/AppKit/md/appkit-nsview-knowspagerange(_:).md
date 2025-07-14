

- AppKit
- NSView
-  knowsPageRange(\_:) 

Instance Method

# knowsPageRange(\_:)

Returns true if the view handles page boundaries, false otherwise.

macOS

``` source
@MainActor
func knowsPageRange(_ range: NSRangePointer) -> Bool
```

## Parameters 

`range`  

On return, holds the page range if true is returned directly. Page numbers are one-based—that is pages run from one to *N*.

## Discussion

Returns false if the view uses the default auto-pagination mechanism. The default implementation returns false. Override this method if your class handles page boundaries.

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

func rectForPage(Int) -> NSRect

Implemented by subclasses to determine the portion of the view to be printed for the specified page number.

func locationOfPrintRect(NSRect) -> NSPoint

Invoked by printView(_:) to determine the location of the region of the view being printed on the physical page.

