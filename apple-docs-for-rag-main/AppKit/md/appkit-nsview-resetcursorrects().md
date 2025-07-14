

- AppKit
- NSView
-  resetCursorRects() 

Instance Method

# resetCursorRects()

Overridden by subclasses to define their default cursor rectangles.

macOS

``` source
@MainActor
func resetCursorRects()
```

## Discussion

A subclass’s implementation must invoke addCursorRect(_:cursor:) for each cursor rectangle it wants to establish. The default implementation does nothing.

Application code should never invoke this method directly; it’s invoked automatically as described in “Responding to User Events and Actions.” Use the invalidateCursorRects(for:) method instead to explicitly rebuild cursor rectangles.

## See Also

### Related Documentation

var visibleRect: NSRect

The portion of the view that isn’t clipped by its superviews.

### Responding to Cursor Movements

func addCursorRect(NSRect, cursor: NSCursor)

Establishes the cursor to be used when the mouse pointer lies within a specified region.

func removeCursorRect(NSRect, cursor: NSCursor)

Completely removes a cursor rectangle from the view.

func discardCursorRects()

Invalidates all cursor rectangles set up using addCursorRect(_:cursor:).

