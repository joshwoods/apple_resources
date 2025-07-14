

- Assignables
- AssignableDocument
- AssignableDocument.Question
- AssignableDocument.Question.Thumbnail
-  AssignableDocument.Question.Thumbnail.Data 

Structure

# AssignableDocument.Question.Thumbnail.Data

A type that contains thumbnail properties.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct Data
```

## Topics

### Inspecting thumbnail data

var box: AssignableDocument.QuestionBox

A copy of the box on the page this thumbnail was generated from.

var image: UIImage

The thumbnail image of the question.

var pageID: AssignableDocument.Page.ID

The ID of the page this thumbnail was generated from.

## See Also

### Inspecting a thumbnail

var data: AssignableDocument.Question.Thumbnail.Data?

The properties of the thumbnail.

var questionID: AssignableDocument.Question.ID

The ID of the question this is for.

