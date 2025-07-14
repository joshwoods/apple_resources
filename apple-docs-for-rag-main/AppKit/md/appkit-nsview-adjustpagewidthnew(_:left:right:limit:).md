

- AppKit
- NSView
-  adjustPageWidthNew(\_:left:right:limit:) 

Instance Method

# adjustPageWidthNew(\_:left:right:limit:)

Overridden by subclasses to adjust page width during automatic pagination.

macOS

``` source
@MainActor
func adjustPageWidthNew(
    _ newRight: UnsafeMutablePointer,
    left oldLeft: CGFloat,
    right oldRight: CGFloat,
    limit rightLimit: CGFloat
)
```

## Parameters 

`newRight`  

Returns by indirection a new CGFloat value for the right edge of the pending page rectangle in the view’s coordinate system.

`oldLeft`  

A CGFloat value that sets the left edge of the pending page rectangle in the view’s coordinate system.

`oldRight`  

A CGFloat value that sets the right edge of the pending page rectangle in the view’s coordinate system.

`rightLimit`  

The leftmost CGFloat value `newRight` can be set to, as calculated using the value of the widthAdjustLimit property.

## Discussion

This method is invoked by printView(_:). The view can pull in the right edge and return the new value in `newRight`, allowing it to prevent items such as small images or text columns from being divided across pages. If `rightLimit` is exceeded, the pagination mechanism simply uses `rightLimit` for the right edge.

The default implementation of this method propagates the message to its subviews, allowing nested views to adjust page width for their drawing as well. An NSButton object or other small view, for example, will nudge the right edge out if necessary to prevent itself from being cut in two (thereby pushing it onto an adjacent page). Subclasses should invoke `super`’s implementation, if desired, after first making their own adjustments.

## See Also

### Handling Pagination

var heightAdjustLimit: CGFloat

The fraction of the page that can be pushed onto the next page during automatic pagination to prevent items such as lines of text from being divided across pages.

var widthAdjustLimit: CGFloat

The fraction of the page that can be pushed onto the next page during automatic pagination to prevent items such as small images or text columns from being divided across pages.

func adjustPageHeightNew(UnsafeMutablePointer&lt;CGFloat>, top: CGFloat, bottom: CGFloat, limit: CGFloat)

Overridden by subclasses to adjust page height during automatic pagination.

func knowsPageRange(NSRangePointer) -> Bool

Returns true if the view handles page boundaries, false otherwise.

func rectForPage(Int) -> NSRect

Implemented by subclasses to determine the portion of the view to be printed for the specified page number.

func locationOfPrintRect(NSRect) -> NSPoint

Invoked by printView(_:) to determine the location of the region of the view being printed on the physical page.

