

- Assignables
-  DocumentElementID 

Protocol

# DocumentElementID

An identifier for an element in a document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
protocol DocumentElementID : Decodable, Encodable, Hashable
```

## Topics

### Implementing an element identifier

associatedtype Element : DocumentElement

The document element type that this reference is for.

**Required**

## Relationships

### Inherits From

- Decodable
- Encodable
- Equatable
- Hashable

### Conforming Types

- AssignableDocument.Page.ID
- AssignedWorkDocument.Page.ID
- BasicDocumentElementID

## See Also

### Document elements

protocol DocumentElement

Represents an element that is contained within a document. Such elements can have identifiers that uniquely identify them within a document.

struct BasicDocumentElementID

A default implementation for a document element identifier.

protocol AssignableDocumentElement

An element of an AssignableDocument.

protocol AssignedWorkDocumentElement

An element of an AssignedWorkDocument.

