

- AppKit
- NSBrowser
-  getRow(\_:column:for:) 

Instance Method

# getRow(\_:column:for:)

Gets the row and column coordinates for the specified point, if a cell exists at that point.

macOS 10.6+

``` source
@MainActor
func getRow(
    _ row: UnsafeMutablePointer?,
    column: UnsafeMutablePointer?,
    for point: NSPoint
) -> Bool
```

## Parameters 

`row`  

On output, the row number of the cell at the specified point, or `-1` if there is no cell at the point.

`column`  

On output, he column number of the cell at the specified point, or `-1` if there is no cell at the point.

`point`  

The point to test.

## Return Value

true if a cell exists at the specified point; otherwise, false.

## Discussion

If a row does not exist at `point`, then `-1` is set for the row. If a column does not exist at `point`, then `-1` is set for the column.

## See Also

### Getting Row Frames

func frame(ofRow: Int, inColumn: Int) -> NSRect

Returns the frame of the cell at the specified location, including the expandable arrow.

