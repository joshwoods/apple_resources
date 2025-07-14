

- SwiftUI
- Table
-  init(\_:children:sortOrder:columnCustomization:columns:) 

Initializer

# init(\_:children:sortOrder:columnCustomization:columns:)

Creates a sortable, hierarchical table that computes its rows based on a collection of identifiable data and key path to the children of that data.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
init(
    _ data: Data,
    children: KeyPath,
    sortOrder: Binding,
    columnCustomization: Binding>? = nil,
    @TableColumnBuilder columns: () -> Columns
) where Rows == TableOutlineGroupContent, Data : RandomAccessCollection, Sort : SortComparator, Columns.TableRowValue == Data.Element, Data.Element == Sort.Compared
```

Available when `Value` is `Rows.TableRowValue`, `Rows` conforms to `TableRowContent`, `Columns` conforms to `TableColumnContent`, and `Rows.TableRowValue` is `Columns.TableRowValue`.

## Parameters 

`data`  

The identifiable data for computing the table rows.

`children`  

A key path to a property whose non-`nil` value gives the children of `data`, and whose `nil` value represents a leaf row of the hierarchy, which is not capable of having children.

`sortOrder`  

A binding to the ordered sorting of columns.

`columnCustomization`  

A binding to the state of columns.

`columns`  

The columns to display in the table.

## Discussion

Each column in the table that should participate in customization is required to have an identifier, specified with customizationID(_:).

## See Also

### Creating a hierarchical table

init&lt;Data>(Data, children: KeyPath&lt;Value, Data?>, columnCustomization: Binding&lt;TableColumnCustomization&lt;Value>>?, columns: () -> Columns)

Creates a hierarchical table that computes its rows based on a collection of identifiable data and key path to the children of that data.

init(_:children:selection:columnCustomization:columns:)

Creates a hierarchical table that computes its rows based on a collection of identifiable data and key path to the children of that data, and supports selecting multiple rows.

init(_:children:selection:sortOrder:columnCustomization:columns:)

Creates a sortable, hierarchical table that computes its rows based on a collection of identifiable data and key path to the children of that data, and supports selecting multiple rows.

