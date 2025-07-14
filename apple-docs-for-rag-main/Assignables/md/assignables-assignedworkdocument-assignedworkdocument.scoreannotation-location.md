

- Assignables
- AssignedWorkDocument
- AssignedWorkDocument.ScoreAnnotation
-  location 

Instance Property

# location

The location of the score annotation on the associated page.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
var location: CGPoint { get set }
```

## See Also

### Inspecting a score annotation

typealias ID

A type representing the stable identity of this score annotation.

var id: AssignedWorkDocument.ScoreAnnotation.ID

The stable identity of this score annotation.

enum Kind

The kind of a score annotation.

var kind: AssignedWorkDocument.ScoreAnnotation.Kind

The kind of score annotation this is. e.g. Incorrect or correct mark.

var pageID: AssignedWorkDocument.Page.ID?

The ID of the page this score annotation is for.

typealias Document

The document type this element is for.

