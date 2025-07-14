

- Assignables
- AssignableDocument
-  AssignableDocument.Error 

Enumeration

# AssignableDocument.Error

Errors for this document type.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
enum Error
```

## Topics

### Document errors

case invalidURL

The URL provided cannot be converted into a new document.

case otherDocumentIsNotAVariant

The other document to be merged into the current document is not a variant of the current document, so merge isn’t possible.

### Enumeration Cases

case exportFailed(partIDs: [AssignableDocument.PartID])

Export of data from the document failed.

### Default Implementations

Error Implementations

## Relationships

### Conforms To

- Error
- Sendable

## See Also

### Inspecting an assignable document

typealias ID

A type representing the stable identity of this document.

var id: AssignableDocument.ID

The stable identity of this document.

var isMultiPageDocument: Bool

`true`, if this document has more than one page; `false`, otherwise.

var isPartial: Bool

Denotes whether or not this document is a partial one.

enum PartIDs

An enumeration containing the identities of parts managed by this view.

var partIDs: [AssignableDocument.PartID]

Returns a collection of identifiers reflecting the manifest of parts available in the document.

struct Question

A question in the assignable document.

struct QuestionBox

A box on a page for a question.

var questions: [AssignableDocument.Question]

A collection of questions defined for this assignable.

typealias Element

The type for elements of this document. An element is a component of the document such as a page or question.

