

- Assignables
- AssignableDocument
-  exportParts(identifiedBy:) 

Instance Method

# exportParts(identifiedBy:)

Given a set of part identifiers, return a dictionary of part ID to part data.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+visionOS

``` source
func exportParts(identifiedBy partIDs: [AssignableDocument.PartID]) async throws -> [AssignableDocument.PartID : MergeablePartData]
```

## Parameters 

`partIDs`  

An array of part IDs to export. This is treated as a set.

## Return Value

A dictionary of part ID to part data file for the requested parts.

