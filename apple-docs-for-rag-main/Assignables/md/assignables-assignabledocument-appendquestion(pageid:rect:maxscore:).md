

- Assignables
- AssignableDocument
-  appendQuestion(pageID:rect:maxScore:) 

Instance Method

# appendQuestion(pageID:rect:maxScore:)

Creates a new question and appends it to the document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@discardableResult
mutating func appendQuestion(
    pageID: AssignableDocument.Page.ID,
    rect: CGRect,
    maxScore: Double? = nil
) -> AssignableDocument.Question.ID
```

## Parameters 

`pageID`  

The ID of the page to append the question to.

`rect`  

The region of the question on the page.

## Return Value

The newly created question’s ID.

## See Also

### Getting and setting the questions

func questions(on: AssignableDocument.Page.ID) -> [AssignableDocument.Question]

Find questions that exist on the specified page.

func removeQuestion(AssignableDocument.Question.ID) -> AssignableDocument.Question?

Removes a question and its boxes from the document.

