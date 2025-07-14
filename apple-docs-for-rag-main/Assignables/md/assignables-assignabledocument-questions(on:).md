

- Assignables
- AssignableDocument
-  questions(on:) 

Instance Method

# questions(on:)

Find questions that exist on the specified page.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
func questions(on pageID: AssignableDocument.Page.ID) -> [AssignableDocument.Question]
```

## Parameters 

`pageID`  

The identifier of the page that contains the questions being sought.

## Return Value

Questions on the specified page.

## See Also

### Getting and setting the questions

func appendQuestion(pageID: AssignableDocument.Page.ID, rect: CGRect, maxScore: Double?) -> AssignableDocument.Question.ID

Creates a new question and appends it to the document.

func removeQuestion(AssignableDocument.Question.ID) -> AssignableDocument.Question?

Removes a question and its boxes from the document.

