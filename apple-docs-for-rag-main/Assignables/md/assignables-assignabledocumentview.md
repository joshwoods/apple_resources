

- Assignables
-  AssignableDocumentView 

Structure

# AssignableDocumentView

SwiftUI View to display an `AssignableDocument`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@MainActor @preconcurrency
struct AssignableDocumentView
```

## Topics

### Creating a document view

init(document: Binding&lt;AssignableDocumentView.Document>, activePartID: MergeablePartsContainerPartID?, hiddenPartIDs: [MergeablePartsContainerPartID], selectedPageID: Binding&lt;AssignableDocumentView.Document.Page.ID?>?, selectedQuestionID: Binding&lt;AssignableDocumentView.Document.Question.ID?>?, showsPageThumbnails: Bool, isStructureEditingEnabled: Bool)

Displays an `AssignableDocument`.

### Customizing the view

var body: some View

The content and behavior of the view.

typealias Document

The document type that this view presents.

### Initializers

init(document: Binding&lt;AssignableDocumentView.Document>, activePartID: MergeablePartsContainerPartID?, hiddenPartIDs: [MergeablePartsContainerPartID], selectedPageID: Binding&lt;AssignableDocumentView.Document.Page.ID?>?, selectedQuestionID: Binding&lt;AssignableDocumentView.Document.Question.ID?>?, showsPageThumbnails: Bool, isStructureEditingEnabled: Bool, allowsPencilDrawing: Bool, onMarkupActivation: (Bool) -> Void)

Displays an `AssignableDocument`.

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

struct AssignedWorkDocumentView

SwiftUI View to display an `AssignedWorkDocument`

