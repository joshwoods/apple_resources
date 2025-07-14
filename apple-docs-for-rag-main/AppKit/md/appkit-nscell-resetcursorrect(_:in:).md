

- AppKit
- NSCell
-  resetCursorRect(\_:in:) 

Instance Method

# resetCursorRect(\_:in:)

Sets the receiver to show the I-beam cursor while it tracks the mouse.

macOS

``` source
@MainActor
func resetCursorRect(
    _ cellFrame: NSRect,
    in controlView: NSView
)
```

## Parameters 

`cellFrame`  

The rectangle in which to display the I-beam cursor.

`controlView`  

The control that manages the cell.

## Discussion

The receiver must be an enabled and selectable (or editable) text-type cell.

This method is invoked by resetCursorRects() and in general you do not need to call this method unless you have a custom `NSView` that uses a cell.

