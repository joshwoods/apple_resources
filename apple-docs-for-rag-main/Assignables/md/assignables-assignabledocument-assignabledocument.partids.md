

- Assignables
- AssignableDocument
-  AssignableDocument.PartIDs 

Enumeration

# AssignableDocument.PartIDs

An enumeration containing the identities of parts managed by this view.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
enum PartIDs
```

## Topics

### Layer types

static let all: [MergeablePartsContainerPartID]

All part IDs containable by this document.

static let authors: MergeablePartsContainerPartID

The identifier for the part that stores authorship information.

static let base: MergeablePartsContainerPartID

The identifier for the part that contains the base PDF upon which this document is built.

static let instructionMarkup: MergeablePartsContainerPartID

The identifier for the part that stores markup intended to provide additional instructions to takers of the assignable.

static let questionBoxes: MergeablePartsContainerPartID

The identifier for the part that stores question definitions.

### Getting the document type

typealias Document

The document type that this part ID is for.

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

