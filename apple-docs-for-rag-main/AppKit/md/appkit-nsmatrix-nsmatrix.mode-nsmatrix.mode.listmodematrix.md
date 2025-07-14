

- AppKit
- NSMatrix
- NSMatrix.Mode
-  NSMatrix.Mode.listModeMatrix 

Case

# NSMatrix.Mode.listModeMatrix

NSCell objects are highlighted, but don’t track the mouse.

macOS

``` source
case listModeMatrix
```

## See Also

### Constants

case trackModeMatrix

The NSCell objects are asked to track the mouse with trackMouse(with:in:of:untilMouseUp:) whenever the cursor is inside their bounds. No highlighting is performed.

case highlightModeMatrix

An NSCell is highlighted before it’s asked to track the mouse, then unhighlighted when it’s done tracking.

case radioModeMatrix

Selects no more than one NSCell at a time.

