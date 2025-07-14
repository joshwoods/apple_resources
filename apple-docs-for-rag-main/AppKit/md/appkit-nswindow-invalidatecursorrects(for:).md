

- AppKit
- NSWindow
-  invalidateCursorRects(for:) 

Instance Method

# invalidateCursorRects(for:)

Marks as invalid the cursor rectangles of a given view object in the window, so they’ll be set up again when the window becomes key.

macOS

``` source
@MainActor
func invalidateCursorRects(for view: NSView)
```

## Parameters 

`view`  

The view in the window’s view hierarchy.

## Discussion

If the window is current the key window, window resets the cursor rectangles immediately.

## See Also

### Related Documentation

func resetCursorRects()

Overridden by subclasses to define their default cursor rectangles.

### Managing Cursor Rectangles

var areCursorRectsEnabled: Bool

A Boolean value that indicates whether the window’s cursor rectangles are enabled.

func enableCursorRects()

Reenables cursor rectangle management within the window after a disableCursorRects() message.

func disableCursorRects()

Disables all cursor rectangle management within the window.

func discardCursorRects()

Invalidates all cursor rectangles in the window.

func resetCursorRects()

Clears the window’s cursor rectangles and the cursor rectangles of the NSView objects in its view hierarchy.

