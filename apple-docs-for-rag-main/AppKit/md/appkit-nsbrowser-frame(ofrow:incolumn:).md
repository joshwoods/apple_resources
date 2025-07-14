

- AppKit
- NSBrowser
-  frame(ofRow:inColumn:) 

Instance Method

# frame(ofRow:inColumn:)

Returns the frame of the cell at the specified location, including the expandable arrow.

macOS 10.6+

``` source
@MainActor
func frame(
    ofRow row: Int,
    inColumn column: Int
) -> NSRect
```

## Parameters 

`row`  

The row of the cell.

`column`  

The column of the cell.

## Return Value

The frame of the cell, in the NSBrowser coordinate space.

## See Also

### Getting Row Frames

func getRow(UnsafeMutablePointer&lt;Int>?, column: UnsafeMutablePointer&lt;Int>?, for: NSPoint) -> Bool

Gets the row and column coordinates for the specified point, if a cell exists at that point.

