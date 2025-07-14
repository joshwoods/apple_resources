

- Assignables
- AssignedWorkDocument
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

### Inspecting a work document

typealias ID

A type representing the stable identity of this document.

var id: AssignedWorkDocument.ID

The stable identity of this document.

var isMultiPageDocument: Bool

`true`, if this document has more than one page; `false`, otherwise.

enum PartIDs

An enumeration containing the identities of parts managed by this view.

var partIDs: [MergeablePartsContainerPartID]

Returns a collection of identifiers reflecting the manifest of parts available in the document.

var scoreAnnotations: [AssignedWorkDocument.ScoreAnnotation]

The collection of score annotations for this work document. Treated as a multiset. i.e. The order of the elements doesn’t matter and duplicate values are allowed.

var scorers: [AnyUserIdentity]

The identities of users scoring this assigned work. Treated as a set.

enum Error

Errors for this document type.

