

- Assignables
- AssignedWorkDocument
-  partIDs 

Instance Property

# partIDs

Returns a collection of identifiers reflecting the manifest of parts available in the document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
var partIDs: [MergeablePartsContainerPartID] { get }
```

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

var scoreAnnotations: [AssignedWorkDocument.ScoreAnnotation]

The collection of score annotations for this work document. Treated as a multiset. i.e. The order of the elements doesn’t matter and duplicate values are allowed.

var scorers: [AnyUserIdentity]

The identities of users scoring this assigned work. Treated as a set.

enum Error

Errors for this document type.

