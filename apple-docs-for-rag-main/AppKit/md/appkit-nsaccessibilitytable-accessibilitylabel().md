

- AppKit
- NSAccessibilityTable
-  accessibilityLabel() 

Instance Method

# accessibilityLabel()

Returns a short description of the table.

macOS

``` source
func accessibilityLabel() -> String?
```

**Required**

## Return Value

The description of the table.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityLabel property.

Do not include the control’s type in the label (for example, use `Employees`, not `Employees Table`). If possible use a single word. To help ensure that accessibility clients such as VoiceOver read the label with the correct intonation, start this label with a capital letter. Do not put a period at the end. Always localize the label.

## See Also

### Supporting Accessibility

func accessibilityColumnHeaderUIElements() -> [Any]?

Returns the column header accessibility elements for the table.

func accessibilityColumns() -> [Any]?

Returns the column accessibility elements for the table.

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

func setAccessibilitySelectedRows([any NSAccessibilityRow])

Sets the table’s currently selected rows.

func accessibilityHeaderGroup() -> String?

Returns the header group for the table.

Deprecated

