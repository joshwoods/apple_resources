

- Assignables
- AssignableDocument
- AssignableDocument.Question
-  init(pageID:boxes:maxScore:) 

Initializer

# init(pageID:boxes:maxScore:)

Initializes an instance of this object with the given values.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
init(
    pageID: AssignableDocument.Page.ID,
    boxes: [AssignableDocument.QuestionBox],
    maxScore: Double? = nil
)
```

## Parameters 

`pageID`  

The page ID this question is for.

`boxes`  

The question boxes associated with this question. Treated as a set.

`maxScore`  

An optional maximum score value for this question.

