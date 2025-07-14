

- Assignables
- AssignedWorkDocument
-  AssignedWorkDocument.PartIDs 

Enumeration

# AssignedWorkDocument.PartIDs

An enumeration containing the identities of parts managed by this view.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
enum PartIDs
```

## Topics

### Layer types

static let all: [MergeablePartsContainerPartID]

All part IDs containable by this document.

static let assignableDocumentAuthors: MergeablePartsContainerPartID

The identifier for the part that stores authorship information.

static let assignableDocumentBase: MergeablePartsContainerPartID

The identifier for the part that contains the base PDF upon which this document is built.

static let assignableDocumentInstructionMarkup: MergeablePartsContainerPartID

The identifier for the part that stores markup intended to provide additional instructions to takers of the assignable.

static let assignableDocumentQuestionBoxes: MergeablePartsContainerPartID

The identifier for the part that stores question definitions.

static let assignees: MergeablePartsContainerPartID

The identifier for the part that stores takers participating in this document.

static let scoreAnnotations: MergeablePartsContainerPartID

The identifier for the part that stores score annotations.

static let scorerMarkup: MergeablePartsContainerPartID

The identifier for the part that stores markup created by the scorer.

static let scorers: MergeablePartsContainerPartID

The identifier for the part that stores scorers participating in grading this document.

static let takerMarkup: MergeablePartsContainerPartID

The identifier for the part that stores markup created by the taker.

### Getting the document type

typealias Document

The document type that this part ID is for.

## See Also

### Inspecting a work document

typealias ID

A type representing the stable identity of this document.

var id: AssignedWorkDocument.ID

The stable identity of this document.

var isMultiPageDocument: Bool

`true`, if this document has more than one page; `false`, otherwise.

var isPartial: Bool

Denotes whether or not this document is a partial one.

var partIDs: [MergeablePartsContainerPartID]

Returns a collection of identifiers reflecting the manifest of parts available in the document.

var scoreAnnotations: [AssignedWorkDocument.ScoreAnnotation]

The collection of score annotations for this work document. Treated as a multiset. i.e. The order of the elements doesn’t matter and duplicate values are allowed.

var scorers: [AnyUserIdentity]

The identities of users scoring this assigned work. Treated as a set.

enum Error

Errors for this document type.

