

- AppKit
- NSBrowser
-  frame(ofInsideOfColumn:) 

Instance Method

# frame(ofInsideOfColumn:)

Returns the rectangle containing the specified column, not including borders.

macOS

``` source
@MainActor
func frame(ofInsideOfColumn column: Int) -> NSRect
```

## Parameters 

`column`  

The index of the column for which to retrieve the inside frame.

## Return Value

The rectangle containing the column, not including the column borders.

## See Also

### Getting Column Frames

func frame(ofColumn: Int) -> NSRect

Returns the rectangle containing the given column.

