

- Assignables
- AssignableDocument
-  exportBaseAsPDF() 

Instance Method

# exportBaseAsPDF()

Exports the base part of this document to a `PDFDocument`.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
func exportBaseAsPDF() async -> PDFDocument
```

## Return Value

The base part of this document as a `PDFDocument`.

## See Also

### Exporting the parts

func export(partIDs: [AssignableDocument.PartID]) async throws -> [AssignableDocument.PartID : URL]

Given a set of part identifiers, return a dictionary of part ID to data objects for the requested layers.

Deprecated

