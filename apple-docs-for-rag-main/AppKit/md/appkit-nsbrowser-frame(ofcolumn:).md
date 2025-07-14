

- AppKit
- NSBrowser
-  frame(ofColumn:) 

Instance Method

# frame(ofColumn:)

Returns the rectangle containing the given column.

macOS

``` source
@MainActor
func frame(ofColumn column: Int) -> NSRect
```

## Parameters 

`column`  

The index of the column for which to retrieve the frame.

## Return Value

The rectangle containing the specified column.

## See Also

### Getting Column Frames

func frame(ofInsideOfColumn: Int) -> NSRect

Returns the rectangle containing the specified column, not including borders.

