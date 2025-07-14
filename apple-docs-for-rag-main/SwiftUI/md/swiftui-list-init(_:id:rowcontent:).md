

- SwiftUI
- List
-  init(\_:id:rowContent:) 

Initializer

# init(\_:id:rowContent:)

Creates a list that identifies its rows based on a key path to the identifier of the underlying data.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
init(
    _ data: Binding,
    id: KeyPath,
    @ViewBuilder rowContent: @escaping (Binding) -> RowContent
) where Content == ForEach, ID, RowContent>, Data : MutableCollection, Data : RandomAccessCollection, ID : Hashable, RowContent : View, Data.Index : Hashable
```

Available when `SelectionValue` is `Never` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`data`  

The data for populating the list.

`id`  

The key path to the data model’s identifier.

`rowContent`  

A view builder that creates the view for a single row of the list.

## See Also

### Creating a list from enumerated data

init(_:rowContent:)

Creates a list that computes its rows on demand from an underlying collection of identifiable data.

init(_:selection:rowContent:)

Creates a list that computes its rows on demand from an underlying collection of identifiable data, optionally allowing users to select a single row.

init(_:id:selection:rowContent:)

Creates a list that identifies its rows based on a key path to the identifier of the underlying data, optionally allowing users to select a single row.

