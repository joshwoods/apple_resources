

- SwiftUI
- Table
-  init(\_:sortOrder:columnCustomization:columns:) 

Initializer

# init(\_:sortOrder:columnCustomization:columns:)

Creates a sortable table that computes its rows based on a collection of identifiable data and has dynamically customizable columns.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
init(
    _ data: Data,
    sortOrder: Binding,
    columnCustomization: Binding>,
    @TableColumnBuilder columns: () -> Columns
) where Rows == TableForEachContent, Data : RandomAccessCollection, Sort : SortComparator, Columns.TableRowValue == Data.Element, Data.Element == Sort.Compared
```

Available when `Value` is `Rows.TableRowValue`, `Rows` conforms to `TableRowContent`, `Columns` conforms to `TableColumnContent`, and `Rows.TableRowValue` is `Columns.TableRowValue`.

## Parameters 

`data`  

The identifiable data for computing the table rows.

`sortOrder`  

A binding to the ordered sorting of columns.

`columnCustomization`  

A binding to the state of columns.

`columns`  

The columns to display in the table.

## Discussion

Each column in the table that should participate in customization is required to have an identifier, specified with customizationID(_:).

## See Also

### Creating a table with customizable columns

init&lt;Data>(Data, columnCustomization: Binding&lt;TableColumnCustomization&lt;Value>>, columns: () -> Columns)

Creates a table that computes its rows based on a collection of identifiable data and has dynamically customizable columns.

init(_:selection:columnCustomization:columns:)

Creates a table that computes its rows based on a collection of identifiable data, that supports selecting multiple rows, and that has dynamically customizable columns.

init(_:selection:sortOrder:columnCustomization:columns:)

Creates a sortable table that computes its rows based on a collection of identifiable data, supports selecting multiple rows, and has dynamically customizable columns.

