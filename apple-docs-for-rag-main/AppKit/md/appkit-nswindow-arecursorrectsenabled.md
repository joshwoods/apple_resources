

- AppKit
- NSWindow
-  areCursorRectsEnabled 

Instance Property

# areCursorRectsEnabled

A Boolean value that indicates whether the window’s cursor rectangles are enabled.

macOS

``` source
@MainActor
var areCursorRectsEnabled: Bool { get }
```

## Discussion

The value of this property is true when cursor rectangles are enabled; otherwise, false.

## See Also

### Related Documentation

func addCursorRect(NSRect, cursor: NSCursor)

Establishes the cursor to be used when the mouse pointer lies within a specified region.

### Managing Cursor Rectangles

func enableCursorRects()

Reenables cursor rectangle management within the window after a disableCursorRects() message.

func disableCursorRects()

Disables all cursor rectangle management within the window.

func discardCursorRects()

Invalidates all cursor rectangles in the window.

func invalidateCursorRects(for: NSView)

Marks as invalid the cursor rectangles of a given view object in the window, so they’ll be set up again when the window becomes key.

func resetCursorRects()

Clears the window’s cursor rectangles and the cursor rectangles of the NSView objects in its view hierarchy.

