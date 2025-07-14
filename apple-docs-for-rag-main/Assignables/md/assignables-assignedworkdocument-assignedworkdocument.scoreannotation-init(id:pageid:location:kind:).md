

- Assignables
- AssignedWorkDocument
- AssignedWorkDocument.ScoreAnnotation
-  init(id:pageID:location:kind:) 

Initializer

# init(id:pageID:location:kind:)

Initializes an instance of this object with the given values.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
init(
    id: AssignedWorkDocument.ScoreAnnotation.ID,
    pageID: AssignedWorkDocument.Page.ID?,
    location: CGPoint,
    kind: AssignedWorkDocument.ScoreAnnotation.Kind
)
```

## Parameters 

`id`  

The ID of this score annotation.

`pageID`  

The ID of the page that this score annotation is on.

`location`  

The location of the score annotation on the associated page.

`kind`  

The kind of score annotation this is. e.g. Incorrect or correct mark.

