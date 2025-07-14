

- Assignables
- AssignableDocument
- AssignableDocument.Question
-  AssignableDocument.Question.Thumbnail 

Structure

# AssignableDocument.Question.Thumbnail

The thumbnail type for this question.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
struct Thumbnail
```

## Topics

### Inspecting a thumbnail

struct Data

A type that contains thumbnail properties.

var data: AssignableDocument.Question.Thumbnail.Data?

The properties of the thumbnail.

var questionID: AssignableDocument.Question.ID

The ID of the question this is for.

## See Also

### Inspecting a question

var boxes: [AssignableDocument.QuestionBox]

The question boxes on pages that denote question regions. Treated as as set.

typealias ID

A type representing the stable identity of this question.

var id: AssignableDocument.Question.ID

The stable identity of this question.

var maxScore: Double?

An optional manual maximum point value for this question.

typealias Document

The document type this element is for.

