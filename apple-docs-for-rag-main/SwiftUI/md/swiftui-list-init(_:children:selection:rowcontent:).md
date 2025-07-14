

- SwiftUI
- List
-  init(\_:children:selection:rowContent:) 

Initializer

# init(\_:children:selection:rowContent:)

Creates a hierarchical list that computes its rows on demand from a binding to an underlying collection of identifiable data and allowing users to have exactly one row always selected.

macOS 13.0+

``` source
@MainActor @preconcurrency
init(
    _ data: Binding,
    children: WritableKeyPath,
    selection: Binding,
    @ViewBuilder rowContent: @escaping (Binding) -> RowContent
) where Content == OutlineGroup, Data.Element.ID, RowContent, RowContent, DisclosureGroup>, Data : MutableCollection, Data : RandomAccessCollection, RowContent : View, Data.Element : Identifiable
```

Available when `SelectionValue` conforms to `Hashable` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`data`  

The identifiable data for computing the list.

`children`  

A key path to a property whose non-`nil` value gives the children of `data`. A non-`nil` but empty value denotes a node capable of having children that is currently childless, such as an empty directory in a file system. On the other hand, if the property at the key path is `nil`, then `data` is treated as a leaf node in the tree, like a regular file in a file system.

`selection`  

A binding to a non optional selected value.

`rowContent`  

A view builder that creates the view for a single row of the list.

## See Also

### Creating a list from hierarchical data

init(_:children:rowContent:)

Creates a hierarchical list that computes its rows on demand from a binding to an underlying collection of identifiable data.

init(_:id:children:rowContent:)

Creates a hierarchical list that identifies its rows based on a key path to the identifier of the underlying data.

init(_:id:children:selection:rowContent:)

Creates a hierarchical list that identifies its rows based on a key path to the identifier of the underlying data and allowing users to have exactly one row always selected.

