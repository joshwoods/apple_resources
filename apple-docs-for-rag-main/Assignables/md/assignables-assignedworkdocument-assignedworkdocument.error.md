

- Assignables
- AssignedWorkDocument
-  AssignedWorkDocument.Error 

Enumeration

# AssignedWorkDocument.Error

Errors for this document type.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
enum Error
```

## Topics

### Variant error

case otherDocumentIsNotAVariant

The other document to be merged into the current document is not a variant of the current document, so merge isn’t possible.

### Enumeration Cases

case exportFailed(partIDs: [AssignedWorkDocument.PartID])

Export of data from the document failed.

### Default Implementations

Error Implementations

## Relationships

### Conforms To

- Error
- Sendable

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

enum PartIDs

An enumeration containing the identities of parts managed by this view.

var partIDs: [MergeablePartsContainerPartID]

Returns a collection of identifiers reflecting the manifest of parts available in the document.

var scoreAnnotations: [AssignedWorkDocument.ScoreAnnotation]

The collection of score annotations for this work document. Treated as a multiset. i.e. The order of the elements doesn’t matter and duplicate values are allowed.

var scorers: [AnyUserIdentity]

The identities of users scoring this assigned work. Treated as a set.

