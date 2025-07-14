

- Assignables
- AssignableDocument
- AssignableDocument.QuestionBox
-  pageID 

Instance Property

# pageID

A read-only property providing the identifier of the page that owns this question box. If the box is not yet assigned to a page, this value is `nil`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
var pageID: AssignableDocument.Page.ID? { get }
```

