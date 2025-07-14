

- Assignables
-  MergeableDocument 

Protocol

# MergeableDocument

Documents conforming to this protocol can merge several copies of the document into a single document.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
protocol MergeableDocument : MergeablePartsContainer, Identifiable
```

## Topics

### Getting the pages

var pages: [Self.Page]

The collection of pages in this document.

**Required**

associatedtype Page : MergeableDocumentPage

The page type this document contains.

**Required**

### Exporting the layers

func exportToPDF(visibleParts: [Self.PartID]) async -> PDFDocument

Exports the indicated layers of this document into a single `PDFDocument`.

**Required**

### Exporting the thumbnails

func pageThumbnails(visibleParts: [Self.PartID]) async -> [Self.Page.ID : Self.Page.Thumbnail]

Exports thumbnails of each page such that the thumbnails contain the indicated layers.

**Required** Default implementation provided.

### Getting the error type

associatedtype Error : Error

The error type for this type.

**Required**

## Relationships

### Inherits From

- Equatable
- Hashable
- Identifiable
- MergeablePartsContainer

### Conforming Types

- AssignableDocument
- AssignedWorkDocument

## See Also

### Mergeable document

struct MergeablePartsContainerPartID

The ID of a part in a `MergeablePartsContainer`.

protocol MergeableDocumentPage

Types conforming to this protocol indicate that they are a page in a MergeableDocument conforming object.

protocol MergeablePartsContainer

Objects conforming to this protocol allow merging in other replicas of themselves or merging in individual parts of themselves.

struct DocumentThumbnail

A structure that contains an image of an entire page or a portion of a page and the ID of the page the image is from.

