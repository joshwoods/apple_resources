

- AppKit
- NSView
-  adjustPageHeightNew(\_:top:bottom:limit:) 

Instance Method

# adjustPageHeightNew(\_:top:bottom:limit:)

Overridden by subclasses to adjust page height during automatic pagination.

macOS

``` source
@MainActor
func adjustPageHeightNew(
    _ newBottom: UnsafeMutablePointer,
    top oldTop: CGFloat,
    bottom oldBottom: CGFloat,
    limit bottomLimit: CGFloat
)
```

## Parameters 

`newBottom`  

Returns by indirection a new CGFloat value for the bottom edge of the pending page rectangle in the view’s coordinate system.

`oldTop`  

A CGFloat value that sets the top edge of the pending page rectangle in the view’s coordinate system.

`oldBottom`  

A CGFloat value that sets the bottom edge of the pending page rectangle in the view’s coordinate system.

`bottomLimit`  

The topmost CGFloat value `newBottom` can be set to, as calculated using the value of the heightAdjustLimit property.

## Discussion

This method is invoked by printView(_:). The view can raise the bottom edge and return the new value in `newBottom`, allowing it to prevent items such as lines of text from being divided across pages. If `bottomLimit` is exceeded, the pagination mechanism simply uses `bottomLimit` for the bottom edge.

The default implementation of this method propagates the message to its subviews, allowing nested views to adjust page height for their drawing as well. An NSButton object or other small view, for example, will nudge the bottom edge up if necessary to prevent itself from being cut in two (thereby pushing it onto an adjacent page). Subclasses should invoke `super`’s implementation, if desired, after first making their own adjustments.

## See Also

### Handling Pagination

var heightAdjustLimit: CGFloat

The fraction of the page that can be pushed onto the next page during automatic pagination to prevent items such as lines of text from being divided across pages.

var widthAdjustLimit: CGFloat

The fraction of the page that can be pushed onto the next page during automatic pagination to prevent items such as small images or text columns from being divided across pages.

func adjustPageWidthNew(UnsafeMutablePointer&lt;CGFloat>, left: CGFloat, right: CGFloat, limit: CGFloat)

Overridden by subclasses to adjust page width during automatic pagination.

func knowsPageRange(NSRangePointer) -> Bool

Returns true if the view handles page boundaries, false otherwise.

func rectForPage(Int) -> NSRect

Implemented by subclasses to determine the portion of the view to be printed for the specified page number.

func locationOfPrintRect(NSRect) -> NSPoint

Invoked by printView(_:) to determine the location of the region of the view being printed on the physical page.

