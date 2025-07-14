

- SwiftUI
- Table
-  init(\_:selection:columns:) 

Initializer

# init(\_:selection:columns:)

Creates a table that computes its rows based on a collection of identifiable data, and that supports selecting multiple rows.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
init(
    _ data: Data,
    selection: Binding>,
    @TableColumnBuilder columns: () -> Columns
) where Rows == TableForEachContent, Data : RandomAccessCollection, Columns.TableRowValue == Data.Element
```

Available when `Value` is `Rows.TableRowValue`, `Rows` conforms to `TableRowContent`, `Columns` conforms to `TableColumnContent`, and `Rows.TableRowValue` is `Columns.TableRowValue`.

Show all declarations

## Parameters 

`data`  

The identifiable data for computing the table rows.

`selection`  

A binding to a set that identifies selected rows IDs.

`columns`  

The columns to display in the table.

## See Also

### Creating a table from columns

init&lt;Data>(Data, columns: () -> Columns)

Creates a table that computes its rows based on a collection of identifiable data.

