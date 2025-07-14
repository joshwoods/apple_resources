

- Assignables
- AssignableDocument
-  export(partIDs:) Deprecated

Instance Method

# export(partIDs:)

Given a set of part identifiers, return a dictionary of part ID to data objects for the requested layers.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
func export(partIDs: [AssignableDocument.PartID]) async throws -> [AssignableDocument.PartID : URL]
```

Deprecated

Use exportParts(identifiedBy:)

## Parameters 

`partIDs`  

An array of part IDs to export. This is treated as a set.

## Return Value

A dictionary of part ID to URLs of the data stored on disk for the requested parts.

## See Also

### Exporting the parts

func exportBaseAsPDF() async -> PDFDocument

Exports the base part of this document to a `PDFDocument`.

