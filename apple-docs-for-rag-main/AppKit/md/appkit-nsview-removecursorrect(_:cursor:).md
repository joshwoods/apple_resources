

- AppKit
- NSView
-  removeCursorRect(\_:cursor:) 

Instance Method

# removeCursorRect(\_:cursor:)

Completely removes a cursor rectangle from the view.

macOS

``` source
@MainActor
func removeCursorRect(
    _ rect: NSRect,
    cursor object: NSCursor
)
```

## Parameters 

`rect`  

A rectangle defining a region of the view. Must match a value previously specified using addCursorRect(_:cursor:).

`object`  

An object representing a cursor. Must match a value previously specified using addCursorRect(_:cursor:).

## Discussion

You should rarely need to use this method. The resetCursorRects() method, which is called when the cursor rectangles need to be rebuilt, should establish only the cursor rectangles needed. If you implement resetCursorRects() in this way, you can then simply modify the state that resetCursorRects() uses to build its cursor rectangles and then invoke the `NSWindow` method invalidateCursorRects(for:).

## See Also

### Responding to Cursor Movements

func addCursorRect(NSRect, cursor: NSCursor)

Establishes the cursor to be used when the mouse pointer lies within a specified region.

func discardCursorRects()

Invalidates all cursor rectangles set up using addCursorRect(_:cursor:).

func resetCursorRects()

Overridden by subclasses to define their default cursor rectangles.

