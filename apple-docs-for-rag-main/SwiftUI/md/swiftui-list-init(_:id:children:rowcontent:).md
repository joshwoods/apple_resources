

- SwiftUI
- List
-  init(\_:id:children:rowContent:) 

Initializer

# init(\_:id:children:rowContent:)

Creates a hierarchical list that identifies its rows based on a key path to the identifier of the underlying data.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
init(
    _ data: Binding,
    id: KeyPath,
    children: WritableKeyPath,
    @ViewBuilder rowContent: @escaping (Binding) -> RowContent
) where Content == OutlineGroup, ID, RowContent, RowContent, DisclosureGroup>, Data : MutableCollection, Data : RandomAccessCollection, ID : Hashable, RowContent : View
```

Available when `SelectionValue` is `Never` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`data`  

The data for populating the list.

`id`  

The key path to the data model’s identifier.

`children`  

A key path to a property whose non-`nil` value gives the children of `data`. A non-`nil` but empty value denotes a node capable of having children that is currently childless, such as an empty directory in a file system. On the other hand, if the property at the key path is `nil`, then `data` is treated as a leaf node in the tree, like a regular file in a file system.

`rowContent`  

A view builder that creates the view for a single row of the list.

## See Also

### Creating a list from hierarchical data

init(_:children:rowContent:)

Creates a hierarchical list that computes its rows on demand from a binding to an underlying collection of identifiable data.

init(_:children:selection:rowContent:)

Creates a hierarchical list that computes its rows on demand from a binding to an underlying collection of identifiable data and allowing users to have exactly one row always selected.

init(_:id:children:selection:rowContent:)

Creates a hierarchical list that identifies its rows based on a key path to the identifier of the underlying data and allowing users to have exactly one row always selected.

