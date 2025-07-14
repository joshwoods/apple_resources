

- SwiftUI
- Table
-  init(of:selection:columnCustomization:columns:rows:) 

Initializer

# init(of:selection:columnCustomization:columns:rows:)

Creates a table with the given columns and rows that supports selecting multiple rows that generates its data using values of the given type and has dynamically customizable columns.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
init(
    of valueType: Value.Type,
    selection: Binding>,
    columnCustomization: Binding>,
    @TableColumnBuilder columns: () -> Columns,
    @TableRowBuilder rows: () -> Rows
)
```

Available when `Value` is `Rows.TableRowValue`, `Rows` conforms to `TableRowContent`, `Columns` conforms to `TableColumnContent`, and `Rows.TableRowValue` is `Columns.TableRowValue`.

Show all declarations

## Parameters 

`valueType`  

The type of value used to derive the table’s contents.

`selection`  

A binding to a set that identifies the selected rows IDs.

`columnCustomization`  

A binding to the state of columns.

`columns`  

The columns to display in the table.

`rows`  

The rows to display in the table.

## Discussion

Each column in the table that should participate in customization is required to have an identifier, specified with customizationID(_:).

## See Also

### Creating a table with dynamically customizable columns

init(of: Value.Type, columnCustomization: Binding&lt;TableColumnCustomization&lt;Value>>, columns: () -> Columns, rows: () -> Rows)

Creates a table with the given columns and rows that generates its contents using values of the given type and has dynamically customizable columns.

init(of:selection:sortOrder:columnCustomization:columns:rows:)

Creates a sortable table with the given columns and rows that supports selecting multiple rows and dynamically customizable columns.

init&lt;Sort>(of: Value.Type, sortOrder: Binding&lt;[Sort]>, columnCustomization: Binding&lt;TableColumnCustomization&lt;Value>>, columns: () -> Columns, rows: () -> Rows)

Creates a sortable table with the given columns and rows and has dynamically customizable columns.

