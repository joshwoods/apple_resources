

- Assignables
- AssignableDocument
-  removeQuestion(\_:) 

Instance Method

# removeQuestion(\_:)

Removes a question and its boxes from the document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
@discardableResult
mutating func removeQuestion(_ questionID: AssignableDocument.Question.ID) -> AssignableDocument.Question?
```

## Parameters 

`questionID`  

The element to remove.

## See Also

### Getting and setting the questions

func appendQuestion(pageID: AssignableDocument.Page.ID, rect: CGRect, maxScore: Double?) -> AssignableDocument.Question.ID

Creates a new question and appends it to the document.

func questions(on: AssignableDocument.Page.ID) -> [AssignableDocument.Question]

Find questions that exist on the specified page.

