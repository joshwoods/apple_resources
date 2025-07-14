

- AppKit
- NSMatrix
-  resetCursorRects() 

Instance Method

# resetCursorRects()

Resets cursor rectangles so the cursor becomes an I-beam over text cells.

macOS

``` source
@MainActor
func resetCursorRects()
```

## Discussion

This method resets the cursor rectangles by sending resetCursorRect(_:in:) to each cell in the receiver. Any cell that has a cursor rectangle to set up should then send addCursorRect(_:cursor:) back to the receiver.

## See Also

### Related Documentation

func addCursorRect(NSRect, cursor: NSCursor)

Establishes the cursor to be used when the mouse pointer lies within a specified region.

func resetCursorRect(NSRect, in: NSView)

Sets the receiver to show the I-beam cursor while it tracks the mouse.

