

- AppKit
- NSView
-  rectForPage(\_:) 

Instance Method

# rectForPage(\_:)

Implemented by subclasses to determine the portion of the view to be printed for the specified page number.

macOS

``` source
@MainActor
func rectForPage(_ page: Int) -> NSRect
```

## Parameters 

`page`  

An integer indicating a page number. Page numbers are one-based—that is pages run from one to *N*.

## Return Value

A rectangle defining the region of the view to be printed for `pageNumber`. This method returns `NSZeroRect` if `pageNumber` is outside the view’s bounds.

## Discussion

If the view responded true to an earlier knowsPageRange(_:) message, this method is invoked for each page it specified in the out parameters of that message. The view is later made to display this rectangle in order to generate the image for this page.

If an `NSView` object responds false to knowsPageRange(_:), this method isn’t invoked by the printing mechanism.

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

func locationOfPrintRect(NSRect) -> NSPoint

Invoked by printView(_:) to determine the location of the region of the view being printed on the physical page.

