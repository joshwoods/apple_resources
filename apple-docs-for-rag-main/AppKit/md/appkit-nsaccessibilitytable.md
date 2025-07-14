

- AppKit
-  NSAccessibilityTable 

Protocol

# NSAccessibilityTable

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a table view.

macOS

``` source
protocol NSAccessibilityTable : NSAccessibilityGroup
```

## Overview

Use this protocol when you want a user interface element to behave like a table—a view that uses a row-and-column format to display a set of related records and their attributes—in the accessibility hierarchy.

You can further enhance the adopting element by implementing any of the information properties or action methods that the NSAccessibilityProtocol protocol declares.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

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

func setAccessibilitySelectedRows([any NSAccessibilityRow])

Sets the table’s currently selected rows.

func accessibilityHeaderGroup() -> String?

Returns the header group for the table.

Deprecated

## Relationships

### Inherits From

- NSAccessibilityElementProtocol
- NSAccessibilityGroup
- NSObjectProtocol

### Inherited By

- NSAccessibilityList
- NSAccessibilityOutline

### Conforming Types

- NSOutlineView
- NSTableView

## See Also

### Lists

protocol NSAccessibilityList

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a list view.

protocol NSAccessibilityOutline

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as an outline view.

protocol NSAccessibilityRow

A role-based protocol that declares the minimum interface necessary for an accessibility element to act as a row for a table, list, or outline view.

