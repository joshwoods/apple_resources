

- AppKit
- NSAccessibilityProtocol
-  accessibilityCell(forColumn:row:) 

Instance Method

# accessibilityCell(forColumn:row:)

Returns the cell at the specified column and row.

macOS 10.10+

``` source
func accessibilityCell(
    forColumn column: Int,
    row: Int
) -> Any?
```

**Required**

## Parameters 

`column`  

The column index.

`row`  

The row index.

## Return Value

The cell specified by the column and row indexes.

## Discussion

This property is required for all elements that function as cell-based tables.

## See Also

### Configuring Cell-Based Tables

func accessibilityColumnIndexRange() -> NSRange

Returns the column index range of the cell.

**Required**

func setAccessibilityColumnIndexRange(NSRange)

Sets the column index range of the cell.

**Required**

func accessibilityRowIndexRange() -> NSRange

Returns the row index range of the cell.

**Required**

func setAccessibilityRowIndexRange(NSRange)

Sets the row index range of the cell.

**Required**

func accessibilitySelectedCells() -> [Any]?

Returns the currently selected cells for the table.

**Required**

func setAccessibilitySelectedCells([Any]?)

Sets the currently selected cells for the table.

**Required**

func accessibilityVisibleCells() -> [Any]?

Returns the visible cells for the table.

**Required**

func setAccessibilityVisibleCells([Any]?)

Sets the visible cells for the table.

**Required**

