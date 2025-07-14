

- Assignables
- AssignedWorkDocumentView
-  init(document:activePartID:hiddenPartIDs:selectedPageID:selectedQuestionID:showsPageThumbnails:isStructureEditingEnabled:onMarkupActivation:) 

Initializer

# init(document:activePartID:hiddenPartIDs:selectedPageID:selectedQuestionID:showsPageThumbnails:isStructureEditingEnabled:onMarkupActivation:)

Displays an `AssignedWorkDocument`.

iOS 18.1+iPadOS 18.1+Mac Catalyst 18.1+

``` source
@MainActor @preconcurrency
init(
    document: Binding,
    activePartID: MergeablePartsContainerPartID? = nil,
    hiddenPartIDs: [MergeablePartsContainerPartID],
    selectedPageID: Binding? = nil,
    selectedQuestionID: Binding? = nil,
    showsPageThumbnails: Bool = true,
    isStructureEditingEnabled: Bool = false,
    onMarkupActivation: @escaping (Bool) -> Void
)
```

## Parameters 

`document`  

A binding to the AssignedWorkDocumentView.Document to present in the view.

`activePartID`  

The `PartID` to enable user interaction on.

`hiddenPartIDs`  

A set of `PartID`s to hide on this view. Treated as a set.

`selectedPageID`  

A binding to the selected page.

`selectedQuestionID`  

A binding to the selected question.

`showsPageThumbnails`  

Controls showing or hiding the document pages thumbnail previews.

`isStructureEditingEnabled`  

Controls access to actions that allow changing the structure of the document on the page thumbnail view contextual menu (i.e. add/duplicate/move/remove pages).

`onMarkupActivation`  

An action performed when the user started or ended a drawing sequence with an Apple Pencil.

