

- SwiftUI
- Table
-  init(of:columns:rows:) 

Initializer

# init(of:columns:rows:)

Creates a table with the given columns and rows that generates its contents using values of the given type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 12.0+visionOS 1.0+

``` source
nonisolated
init(
    of valueType: Value.Type,
    @TableColumnBuilder columns: () -> Columns,
    @TableRowBuilder rows: () -> Rows
)
```

Available when `Value` is `Rows.TableRowValue`, `Rows` conforms to `TableRowContent`, `Columns` conforms to `TableColumnContent`, and `Rows.TableRowValue` is `Columns.TableRowValue`.

## Parameters 

`valueType`  

The type of value used to derive the table’s contents.

`columns`  

The columns to display in the table.

`rows`  

The rows to display in the table.

## See Also

### Creating a table from columns and rows

init(of:selection:columns:rows:)

Creates a table with the given columns and rows that supports selecting multiple rows that generates its data using values of the given type.

