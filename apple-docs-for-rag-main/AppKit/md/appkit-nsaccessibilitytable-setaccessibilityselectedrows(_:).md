

- AppKit
- NSAccessibilityTable
-  setAccessibilitySelectedRows(\_:) 

Instance Method

# setAccessibilitySelectedRows(\_:)

Sets the table’s currently selected rows.

macOS

``` source
optional func setAccessibilitySelectedRows(_ selectedRows: [any NSAccessibilityRow])
```

## Parameters 

`selectedRows`  

An array containing the row elements to be selected.

## Discussion

This method is the setter for the NSAccessibilityProtocol protocol’s accessibilitySelectedRows property. Implementing this method allows the user to change the selected row using an accessibility client. Additionally, your class needs to send a selectedRowsChanged notification whenever the table’s selected rows change.

## See Also

### Supporting Accessibility

func accessibilityColumnHeaderUIElements() -> [Any]?

Returns the column header accessibility elements for the table.

func accessibilityColumns() -> [Any]?

Returns the column accessibility elements for the table.

func accessibilityLabel() -> String?

Returns a short description of the table.

**Required**

func accessibilityRowHeaderUIElements() -> [Any]?

Returns the row header accessibility elements for the table.

func accessibilityRows() -> [any NSAccessibilityRow]?

Returns the row accessibility elements for the table.

**Required**

func accessibilitySelectedCells() -> [Any]?

The currently selected cells for the table.

func accessibilitySelectedColumns() -> [Any]?

Returns the currently selected columns for the table.

func accessibilitySelectedRows() -> [any NSAccessibilityRow]?

Returns the currently selected rows for the table.

func accessibilityVisibleCells() -> [Any]?

Returns the visible cells for the table.

func accessibilityVisibleColumns() -> [Any]?

Returns the visible columns for the table.

func accessibilityVisibleRows() -> [any NSAccessibilityRow]?

Returns the visible rows for the table.

func accessibilityHeaderGroup() -> String?

Returns the header group for the table.

Deprecated

