

- Assignables
-  DocumentElement 

Protocol

# DocumentElement

Represents an element that is contained within a document. Such elements can have identifiers that uniquely identify them within a document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
protocol DocumentElement : Hashable
```

## Topics

### Implementing a document element

associatedtype Document : MergeableDocument

The document type this element is for.

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable

### Inherited By

- AssignableDocumentElement
- AssignedWorkDocumentElement

### Conforming Types

- AssignableDocument.Page
- AssignableDocument.Question
- AssignableDocument.QuestionBox
- AssignedWorkDocument.Page
- AssignedWorkDocument.ScoreAnnotation

## See Also

### Document elements

struct BasicDocumentElementID

A default implementation for a document element identifier.

protocol DocumentElementID

An identifier for an element in a document.

protocol AssignableDocumentElement

An element of an AssignableDocument.

protocol AssignedWorkDocumentElement

An element of an AssignedWorkDocument.

