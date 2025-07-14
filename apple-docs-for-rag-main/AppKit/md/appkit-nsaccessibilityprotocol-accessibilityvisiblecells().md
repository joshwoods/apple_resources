

- AppKit
- NSAccessibilityProtocol
-  accessibilityVisibleCells() 

Instance Method

# accessibilityVisibleCells()

Returns the visible cells for the table.

macOS 10.10+

``` source
func accessibilityVisibleCells() -> [Any]?
```

**Required**

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

func setAccessibilityVisibleCells([Any]?)

Sets the visible cells for the table.

**Required**

func accessibilityCell(forColumn: Int, row: Int) -> Any?

Returns the cell at the specified column and row.

**Required**

