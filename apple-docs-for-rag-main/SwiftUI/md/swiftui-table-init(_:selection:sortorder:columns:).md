

- SwiftUI
- Table
-  init(\_:selection:sortOrder:columns:) 

Initializer

# init(\_:selection:sortOrder:columns:)

Creates a sortable table that computes its rows based on a collection of identifiable data, and supports selecting multiple rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
init(
    _ data: Data,
    selection: Binding>,
    sortOrder: Binding,
    @TableColumnBuilder columns: () -> Columns
) where Rows == TableForEachContent, Data : RandomAccessCollection, Sort : SortComparator, Columns.TableRowValue == Data.Element, Data.Element == Sort.Compared
```

Available when `Value` is `Rows.TableRowValue`, `Rows` conforms to `TableRowContent`, `Columns` conforms to `TableColumnContent`, and `Rows.TableRowValue` is `Columns.TableRowValue`.

Show all declarations

## Parameters 

`data`  

The identifiable data for computing the table rows.

`selection`  

A binding to a set that identifies selected rows IDs.

`sortOrder`  

A binding to the ordered sorting of columns.

`columns`  

The columns to display in the table.

## See Also

### Creating a sortable table from columns

init&lt;Data, Sort>(Data, sortOrder: Binding&lt;[Sort]>, columns: () -> Columns)

Creates a sortable table that computes its rows based on a collection of identifiable data.

