

- Assignables
- AssignedWorkDocumentView
-  init(document:activePartID:hiddenPartIDs:selectedPageID:selectedQuestionID:showsPageThumbnails:isStructureEditingEnabled:) 

Initializer

# init(document:activePartID:hiddenPartIDs:selectedPageID:selectedQuestionID:showsPageThumbnails:isStructureEditingEnabled:)

Displays an `AssignedWorkDocument`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@MainActor @preconcurrency
init(
    document: Binding,
    activePartID: MergeablePartsContainerPartID? = nil,
    hiddenPartIDs: [MergeablePartsContainerPartID],
    selectedPageID: Binding? = nil,
    selectedQuestionID: Binding? = nil,
    showsPageThumbnails: Bool = true,
    isStructureEditingEnabled: Bool = false
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

## Discussion

- Example:

```
    AssignedWorkDocumentView(
        document: $document,
        activePartID: activeLayerID,
        hiddenPartIDs: hiddenPartIDs,
        selectedPageID: $selectedPageID,
        showsPageThumbnails: isMultiPageDocument,
        isStructureEditingEnabled: false,
        onMarkupActivation: { isMarkupActivated in
            if isMarkupActivated {
                activeLayerID = AssignedWorkDocument.PartIDs.scorerMarkup
                isMarkupSelected = true
            }
        }
    )
```

