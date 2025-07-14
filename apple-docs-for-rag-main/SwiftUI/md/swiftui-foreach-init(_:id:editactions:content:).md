

- SwiftUI
- ForEach
-  init(\_:id:editActions:content:) 

Initializer

# init(\_:id:editActions:content:)

Creates an instance that uniquely identifies and creates views across updates based on the identity of the underlying data.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    _ data: Binding,
    id: KeyPath,
    editActions: EditActions,
    @ViewBuilder content: @escaping (Binding) -> R
) where Data == IndexedIdentifierCollection, Content == EditableCollectionContent, C : MutableCollection, C : RandomAccessCollection, R : View, C.Index : Hashable
```

Available when `Data` conforms to `RandomAccessCollection` and `ID` conforms to `Hashable`.

## Parameters 

`data`  

The identified data that the ForEach instance uses to create views dynamically and can be edited by the user.

`id`  

The key path to the provided data’s identifier.

`editActions`  

The edit actions that are synthesized on `data`.

`content`  

The view builder that creates views dynamically.

## Discussion

It’s important that the `id` of a data element doesn’t change unless you replace the data element with a new data element that has a new identity. If the `id` of a data element changes, the content view generated from that data element loses any current state and animations.

When placed inside a `List` the edit actions (like delete or move) can be automatically synthesized by specifying an appropriate `EditActions`.

The following example shows a list of recipes whose elements can be deleted and reordered:

```
List {
    ForEach($recipes, editActions: [.delete, .move]) { $recipe in
        RecipeCell($recipe)
    }
}
```

Use deleteDisabled(_:) and moveDisabled(_:) to disable respectively delete or move actions on a per-row basis.

The following example shows a list of recipes whose elements can be deleted only if they satisfy a condition:

```
List {
    ForEach($recipes, editActions: .delete) { $recipe in
        RecipeCell($recipe)
            .deleteDisabled(recipe.isFromMom)
    }
}
```

Explicit `DynamicViewContent.onDelete(perform:)`, `DynamicViewContent.onMove(perform:)`, or `View.swipeActions(edge:allowsFullSwipe:content:)` modifiers will override any synthesized actions. Use this modifier if you need fine-grain control on how mutations are applied to the data driving the `ForEach`. For example, if you need to execute side effects or call into your existing model code.

## See Also

### Creating an editable collection

init&lt;C, R>(Binding&lt;C>, editActions: EditActions&lt;C>, content: (Binding&lt;C.Element>) -> R)

Creates an instance that uniquely identifies and creates views across updates based on the identity of the underlying data.

