

- Assignables
-  AssignedWorkDocumentView 

Structure

# AssignedWorkDocumentView

SwiftUI View to display an `AssignedWorkDocument`

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@MainActor @preconcurrency
struct AssignedWorkDocumentView
```

## Topics

### Creating a document view

init(document: Binding&lt;AssignedWorkDocumentView.Document>, activePartID: MergeablePartsContainerPartID?, hiddenPartIDs: [MergeablePartsContainerPartID], selectedPageID: Binding&lt;AssignedWorkDocumentView.Document.Page.ID?>?, selectedQuestionID: Binding&lt;AssignableDocument.Question.ID?>?, showsPageThumbnails: Bool, isStructureEditingEnabled: Bool)

Displays an `AssignedWorkDocument`.

### Implementing a view

var body: some View

The content and behavior of the view.

typealias Document

The document type that this view presents.

### Initializers

init(document: Binding&lt;AssignedWorkDocumentView.Document>, activePartID: MergeablePartsContainerPartID?, hiddenPartIDs: [MergeablePartsContainerPartID], selectedPageID: Binding&lt;AssignedWorkDocumentView.Document.Page.ID?>?, selectedQuestionID: Binding&lt;AssignableDocument.Question.ID?>?, showsPageThumbnails: Bool, isStructureEditingEnabled: Bool, onMarkupActivation: (Bool) -> Void)

Displays an `AssignedWorkDocument`.

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Presentation

struct AssignableDocumentView

SwiftUI View to display an `AssignableDocument`.

