

- Assignables
- AssignableDocument
-  isPartial 

Instance Property

# isPartial

Denotes whether or not this document is a partial one.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
var isPartial: Bool { get }
```

## Discussion

Documents are considered partial when they are reconstituted with some, not all, of their parts. When a document is considered partial, you cannot read or write to its missing parts.

## See Also

### Inspecting an assignable document

typealias ID

A type representing the stable identity of this document.

var id: AssignableDocument.ID

The stable identity of this document.

var isMultiPageDocument: Bool

`true`, if this document has more than one page; `false`, otherwise.

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

enum Error

Errors for this document type.

