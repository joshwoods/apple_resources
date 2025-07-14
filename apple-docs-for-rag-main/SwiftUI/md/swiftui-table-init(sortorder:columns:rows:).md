

- SwiftUI
- Table
-  init(sortOrder:columns:rows:) 

Initializer

# init(sortOrder:columns:rows:)

Creates a sortable table with the given columns and rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
init(
    sortOrder: Binding,
    @TableColumnBuilder columns: () -> Columns,
    @TableRowBuilder rows: () -> Rows
) where Sort : SortComparator, Columns.TableRowValue == Sort.Compared
```

Available when `Value` is `Rows.TableRowValue`, `Rows` conforms to `TableRowContent`, `Columns` conforms to `TableColumnContent`, and `Rows.TableRowValue` is `Columns.TableRowValue`.

## Parameters 

`sortOrder`  

A binding to the ordered sorting of columns.

`columns`  

The columns to display in the table.

`rows`  

The rows to display in the table.

## See Also

### Creating a sortable table from columns and rows

init&lt;Sort>(of: Value.Type, sortOrder: Binding&lt;[Sort]>, columns: () -> Columns, rows: () -> Rows)

Creates a sortable table with the given columns and rows.

init(of:selection:sortOrder:columns:rows:)

Creates a sortable table with the given columns and rows that supports selecting multiple rows.

init(selection:sortOrder:columns:rows:)

Creates a sortable table with the given columns and rows that supports selecting multiple rows.

