

- SwiftUI
- List
-  init(\_:selection:rowContent:) 

Initializer

# init(\_:selection:rowContent:)

Creates a list that computes its rows on demand from an underlying collection of identifiable data, optionally allowing users to select a single row.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
init(
    _ data: Binding,
    selection: Binding?,
    @ViewBuilder rowContent: @escaping (Binding) -> RowContent
) where Content == ForEach, Data.Element.ID, RowContent>, Data : MutableCollection, Data : RandomAccessCollection, RowContent : View, Data.Element : Identifiable, Data.Index : Hashable
```

Available when `SelectionValue` conforms to `Hashable` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`data`  

The identifiable data for computing the list.

`selection`  

A binding to a selected value.

`rowContent`  

A view builder that creates the view for a single row of the list.

## See Also

### Creating a list from enumerated data

init(_:rowContent:)

Creates a list that computes its rows on demand from an underlying collection of identifiable data.

init(_:id:rowContent:)

Creates a list that identifies its rows based on a key path to the identifier of the underlying data.

init(_:id:selection:rowContent:)

Creates a list that identifies its rows based on a key path to the identifier of the underlying data, optionally allowing users to select a single row.

