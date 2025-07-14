

- SwiftUI
- List
-  init(\_:id:editActions:rowContent:) 

Initializer

# init(\_:id:editActions:rowContent:)

Creates a list that computes its rows on demand from an underlying collection of identifiable data and allows to edit the collection.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
init(
    _ data: Binding,
    id: KeyPath,
    editActions: EditActions,
    @ViewBuilder rowContent: @escaping (Binding) -> RowContent
) where Content == ForEach, ID, EditableCollectionContent>, Data : MutableCollection, Data : RandomAccessCollection, ID : Hashable, RowContent : View, Data.Index : Hashable
```

Available when `SelectionValue` is `Never` and `Content` conforms to `View`.

## Parameters 

`data`  

A collection of identifiable data for computing the list.

`id`  

The key path to the data model’s identifier.

`editActions`  

The edit actions that are synthesized on `data`.

`rowContent`  

A view builder that creates the view for a single row of the list.

## Discussion

The following example creates a list to display a collection of favorite foods allowing the user to delete or move elements from the collection.

```
List($foods, editActions: [.delete, .move]) { $food in
   HStack {
       Text(food.name)
       Toggle("Favorite", isOn: $food.isFavorite)
   }
}
```

Use deleteDisabled(_:) and moveDisabled(_:) to disable respectively delete or move actions on a per-row basis.

Explicit `DynamicViewContent.onDelete(perform:)`, `DynamicViewContent.onMove(perform:)`, or `View.swipeActions(edge:allowsFullSwipe:content:)` modifiers will override any synthesized action

## See Also

### Creating a list from editable data

init&lt;Data, RowContent>(Binding&lt;Data>, editActions: EditActions&lt;Data>, rowContent: (Binding&lt;Data.Element>) -> RowContent)

Creates a list that computes its rows on demand from an underlying collection of identifiable data and allows to edit the collection.

init(_:editActions:selection:rowContent:)

Creates a list that computes its rows on demand from an underlying collection of identifiable data, allows to edit the collection, and requires a selection of a single row.

init(_:id:editActions:selection:rowContent:)

Creates a list that computes its rows on demand from an underlying collection of identifiable, allows to edit the collection, and requires a selection of a single row.

