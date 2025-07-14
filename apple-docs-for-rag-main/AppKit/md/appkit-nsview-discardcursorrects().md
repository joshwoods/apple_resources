

- AppKit
- NSView
-  discardCursorRects() 

Instance Method

# discardCursorRects()

Invalidates all cursor rectangles set up using addCursorRect(_:cursor:).

macOS

``` source
@MainActor
func discardCursorRects()
```

## Discussion

You need never invoke this method directly; neither is it typically invoked during the invalidation of cursor rectangles. NSWindow automatically invalidates cursor rectangles in response to invalidateCursorRects(for:) and before the view’s cursor rectangles are reestablished using resetCursorRects(). This method is invoked just before the view is removed from a window and when the view is deallocated.

## See Also

### Related Documentation

func discardCursorRects()

Invalidates all cursor rectangles in the window.

### Responding to Cursor Movements

func addCursorRect(NSRect, cursor: NSCursor)

Establishes the cursor to be used when the mouse pointer lies within a specified region.

func removeCursorRect(NSRect, cursor: NSCursor)

Completely removes a cursor rectangle from the view.

func resetCursorRects()

Overridden by subclasses to define their default cursor rectangles.

