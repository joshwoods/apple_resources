

- Assignables
- AssignableDocumentView
-  init(document:activePartID:hiddenPartIDs:selectedPageID:selectedQuestionID:showsPageThumbnails:isStructureEditingEnabled:allowsPencilDrawing:onMarkupActivation:) 

Initializer

# init(document:activePartID:hiddenPartIDs:selectedPageID:selectedQuestionID:showsPageThumbnails:isStructureEditingEnabled:allowsPencilDrawing:onMarkupActivation:)

Displays an `AssignableDocument`.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+

``` source
@MainActor @preconcurrency
init(
    document: Binding,
    activePartID: MergeablePartsContainerPartID? = nil,
    hiddenPartIDs: [MergeablePartsContainerPartID] = [],
    selectedPageID: Binding? = nil,
    selectedQuestionID: Binding? = nil,
    showsPageThumbnails: Bool = true,
    isStructureEditingEnabled: Bool = true,
    allowsPencilDrawing: Bool = true,
    onMarkupActivation: @escaping (Bool) -> Void
)
```

## Parameters 

`document`  

A binding to the AssignableDocumentView.Document to present in the view.

`activePartID`  

The `PartID` to enable user interaction on.

`hiddenPartIDs`  

A set of `PartID`s to hide on this view. Treated as a set.

`selectedPageID`  

A binding to the selected page id.

`selectedQuestionID`  

A binding to the selected question id.

`showsPageThumbnails`  

Controls showing or hiding the document pages thumbnail previews.

`isStructureEditingEnabled`  

Controls access to actions that allow changing the structure of the document on the page thumbnail view contextual menu (i.e. add/duplicate/move/remove pages).

`onMarkupActivation`  

An action performed when the user started or ended a drawing sequence with an Apple Pencil.

