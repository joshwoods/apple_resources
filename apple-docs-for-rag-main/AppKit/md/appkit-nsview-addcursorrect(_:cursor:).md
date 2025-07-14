

- AppKit
- NSView
-  addCursorRect(\_:cursor:) 

Instance Method

# addCursorRect(\_:cursor:)

Establishes the cursor to be used when the mouse pointer lies within a specified region.

macOS

``` source
@MainActor
func addCursorRect(
    _ rect: NSRect,
    cursor object: NSCursor
)
```

## Parameters 

`rect`  

A rectangle defining a region of the view.

`object`  

An object representing a cursor.

## Discussion

Cursor rectangles aren’t subject to clipping by superviews, nor are they intended for use with rotated views. You should explicitly confine a cursor rectangle to the view’s visible rectangle to prevent improper behavior.

This method is intended to be invoked only by the resetCursorRects() method. If invoked in any other way, the resulting cursor rectangle will be discarded the next time the view’s cursor rectangles are rebuilt.

## See Also

### Related Documentation

var visibleRect: NSRect

The portion of the view that isn’t clipped by its superviews.

### Responding to Cursor Movements

func removeCursorRect(NSRect, cursor: NSCursor)

Completely removes a cursor rectangle from the view.

func discardCursorRects()

Invalidates all cursor rectangles set up using addCursorRect(_:cursor:).

func resetCursorRects()

Overridden by subclasses to define their default cursor rectangles.

