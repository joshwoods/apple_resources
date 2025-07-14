

- SwiftUI
- Table
-  init(\_:columns:) 

Initializer

# init(\_:columns:)

Creates a table that computes its rows based on a collection of identifiable data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
init(
    _ data: Data,
    @TableColumnBuilder columns: () -> Columns
) where Rows == TableForEachContent, Data : RandomAccessCollection, Columns.TableRowValue == Data.Element
```

Available when `Value` is `Rows.TableRowValue`, `Rows` conforms to `TableRowContent`, `Columns` conforms to `TableColumnContent`, and `Rows.TableRowValue` is `Columns.TableRowValue`.

## Parameters 

`data`  

The identifiable data for computing the table rows.

`columns`  

The columns to display in the table.

## See Also

### Creating a table from columns

init(_:selection:columns:)

Creates a table that computes its rows based on a collection of identifiable data, and that supports selecting multiple rows.

