

- Assignables
- AssignableDocument
-  questionThumbnails(visibleParts:) 

Instance Method

# questionThumbnails(visibleParts:)

Produces thumbnails of question regions within the document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
func questionThumbnails(visibleParts: [AssignableDocument.PartID]) async -> [AssignableDocument.Question.ID : [AssignableDocument.Question.Thumbnail]]
```

## Parameters 

`visibleParts`  

The parts to display in the thumbnails.

## Return Value

A dictionary of AssignableDocument.Question.ID to array of AssignableDocument.Question.Thumbnail.

