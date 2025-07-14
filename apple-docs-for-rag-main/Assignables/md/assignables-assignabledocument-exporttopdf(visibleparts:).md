

- Assignables
- AssignableDocument
-  exportToPDF(visibleParts:) 

Instance Method

# exportToPDF(visibleParts:)

Exports the indicated parts of this document into a single `PDFDocument`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
func exportToPDF(visibleParts: [MergeablePartsContainerPartID]) async -> PDFDocument
```

## Parameters 

`visibleParts`  

The lDs of parts that should be included in the exported PDF.

