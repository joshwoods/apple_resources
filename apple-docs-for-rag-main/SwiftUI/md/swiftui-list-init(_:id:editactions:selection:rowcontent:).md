

- SwiftUI
- List
-  init(\_:id:editActions:selection:rowContent:) 

Initializer

# init(\_:id:editActions:selection:rowContent:)

Creates a list that computes its rows on demand from an underlying collection of identifiable, allows to edit the collection, and requires a selection of a single row.

macOS 13.0+

``` source
@MainActor @preconcurrency
init(
    _ data: Binding,
    id: KeyPath,
    editActions: EditActions,
    selection: Binding,
    @ViewBuilder rowContent: @escaping (Binding) -> RowContent
) where Content == ForEach, ID, EditableCollectionContent>, Data : MutableCollection, Data : RandomAccessCollection, ID : Hashable, RowContent : View, Data.Index : Hashable
```

Available when `SelectionValue` conforms to `Hashable` and `Content` conforms to `View`.

Show all declarations

## Parameters 

`data`  

The identifiable data for computing and to be edited by the list.

`id`  

The key path to the data model’s identifier.

`editActions`  

The edit actions that are synthesized on `data`.

`selection`  

A binding to a non optional selected value.

`rowContent`  

A view builder that creates the view for a single row of

## Discussion

The following example creates a list to display a collection of favorite foods allowing the user to delete or move elements from the collection, and selects a single row.

```
List(
    $foods,
    editActions: [.delete, .move],
    selection: $selectedFood
) { $food in
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

init&lt;Data, ID, RowContent>(Binding&lt;Data>, id: KeyPath&lt;Data.Element, ID>, editActions: EditActions&lt;Data>, rowContent: (Binding&lt;Data.Element>) -> RowContent)

Creates a list that computes its rows on demand from an underlying collection of identifiable data and allows to edit the collection.

