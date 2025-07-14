

- Assignables
- MergeablePartsContainer
-  export(partIDs:) Deprecated

Instance Method

# export(partIDs:)

Given a set of part identifiers, return a dictionary of part ID to URL to the part data file for the requested parts.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
func export(partIDs: [Self.PartID]) async throws -> [Self.PartID : URL]
```

**Required**

Deprecated

Use exportParts(identifiedBy:)

## Parameters 

`partIDs`  

An array of part IDs to export. This is treated as a set.

## Return Value

A dictionary of part ID to URL to the part data file for the requested parts.

