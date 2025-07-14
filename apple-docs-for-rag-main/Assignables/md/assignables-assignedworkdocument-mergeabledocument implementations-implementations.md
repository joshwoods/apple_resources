

- Assignables
- AssignedWorkDocument
-  MergeableDocument Implementations 

API Collection

# MergeableDocument Implementations

## Topics

### Structures

struct Page

A page within this assigned work document.

### Instance Properties

var pages: [AssignedWorkDocument.Page]

The collection of pages in this document.

### Instance Methods

func exportToPDF(visibleParts: [MergeablePartsContainerPartID]) async -> PDFDocument

Exports the indicated layers of this document into a single `PDFDocument`.

func pageThumbnails(visibleParts: [MergeablePartsContainerPartID]) async -> [Self.Page.ID : Self.Page.Thumbnail]

Exports thumbnails of each page such that the thumbnails contain the indicated layers.

