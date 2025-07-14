

- Assignables
- AssignableDocumentView
-  init(document:activePartID:hiddenPartIDs:selectedPageID:selectedQuestionID:showsPageThumbnails:isStructureEditingEnabled:) 

Initializer

# init(document:activePartID:hiddenPartIDs:selectedPageID:selectedQuestionID:showsPageThumbnails:isStructureEditingEnabled:)

Displays an `AssignableDocument`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@MainActor @preconcurrency
init(
    document: Binding,
    activePartID: MergeablePartsContainerPartID? = nil,
    hiddenPartIDs: [MergeablePartsContainerPartID] = [],
    selectedPageID: Binding? = nil,
    selectedQuestionID: Binding? = nil,
    showsPageThumbnails: Bool = true,
    isStructureEditingEnabled: Bool = true
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

## Discussion

- Example:

```
    AssignableDocumentView(
        document: $document,
        activePartID: activeLayerID,
        hiddenPartIDs: hiddenPartIDs,
        selectedPageID: $selectedPageID,
        showsPageThumbnails: isMultiPageDocument,
        isStructureEditingEnabled: false,
        onMarkupActivation: { isMarkupActivated in
            if isMarkupActivated {
                activeLayerID = AssignableDocument.PartIDs.instructionMarkup
                isMarkupSelected = true
            }
        }
    )
```

