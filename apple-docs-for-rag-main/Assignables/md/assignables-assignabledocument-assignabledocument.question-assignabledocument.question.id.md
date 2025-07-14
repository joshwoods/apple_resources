

- Assignables
- AssignableDocument
- AssignableDocument.Question
-  AssignableDocument.Question.ID 

Type Alias

# AssignableDocument.Question.ID

A type representing the stable identity of this question.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
typealias ID = BasicDocumentElementID
```

## See Also

### Inspecting a question

var boxes: [AssignableDocument.QuestionBox]

The question boxes on pages that denote question regions. Treated as as set.

var id: AssignableDocument.Question.ID

The stable identity of this question.

var maxScore: Double?

An optional manual maximum point value for this question.

struct Thumbnail

The thumbnail type for this question.

typealias Document

The document type this element is for.

