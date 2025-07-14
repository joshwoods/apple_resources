

- Assignables
-  MergeablePartsContainer 

Protocol

# MergeablePartsContainer

Objects conforming to this protocol allow merging in other replicas of themselves or merging in individual parts of themselves.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
protocol MergeablePartsContainer : Hashable
```

## Topics

### Merging the parts

func merge(other: Self) throws -> Bool

Merge another object of this type into this object.

**Required**

Deprecated

### Exporting the parts

func export(partIDs: [Self.PartID]) async throws -> [Self.PartID : URL]

Given a set of part identifiers, return a dictionary of part ID to URL to the part data file for the requested parts.

**Required**

Deprecated

### Getting the part identifiers

var partIDs: [Self.PartID]

Returns a collection of part IDs reflecting the manifest of parts available in the document.

**Required**

typealias PartID

The type for document layer IDs.

### Inspecting the parts

var isPartial: Bool

Documents are considered partial when they are reconstituted missing one or more of their associated document part IDs. When a document is considered partial it is expected that we shouldn’t be able to both read or write to the parts that the document has neither been reconstituted or merged with.

**Required**

### Instance Methods

func exportParts(identifiedBy: [Self.PartID]) async throws -> [Self.PartID : MergeablePartData]

Given a set of part identifiers, return a dictionary of part ID to part data.

**Required**

func makePart(for: Self.PartID) throws -> MergeablePartData?

Creates data for the part with the given identifier.

**Required**

func merge(Self) async throws -> Bool

Merge another object of this type into this object.

**Required**

func merge(partData: MergeablePartData, into: Self.PartID) async throws -> Bool

Merges an individual part into the specified part of this object.

**Required**

func merge(partID: Self.PartID, partDataURL: URL) throws -> Bool

Merges an individual part into the specified part of this object.

**Required**

Deprecated

## Relationships

### Inherits From

- Equatable
- Hashable

### Inherited By

- MergeableDocument

### Conforming Types

- AssignableDocument
- AssignedWorkDocument

## See Also

### Mergeable document

protocol MergeableDocument

Documents conforming to this protocol can merge several copies of the document into a single document.

struct MergeablePartsContainerPartID

The ID of a part in a `MergeablePartsContainer`.

protocol MergeableDocumentPage

Types conforming to this protocol indicate that they are a page in a MergeableDocument conforming object.

struct DocumentThumbnail

A structure that contains an image of an entire page or a portion of a page and the ID of the page the image is from.

