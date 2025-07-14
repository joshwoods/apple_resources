

- Assignables
- AssignableDocument
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Access the question box that the identifier denotes, if any.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
subscript(questionBoxID: AssignableDocument.QuestionBox.ID) -> AssignableDocument.QuestionBox? { get set }
```

## See Also

### Accessing documents

subscript(AssignableDocument.Question.ID) -> AssignableDocument.Question?

Access the question that the identifier denotes, if any.

subscript(AssignableDocument.Page.ID) -> AssignableDocument.Page?

Access the page that the identifier denotes, if any.

