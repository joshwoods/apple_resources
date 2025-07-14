

- Assignables
- AssignedWorkDocument
-  export(partIDs:) Deprecated

Instance Method

# export(partIDs:)

Given a set of part identifiers, return a dictionary of part ID to data objects for the requested parts.

iOS 17.4+iPadOS 17.4+visionOSMac Catalyst 17.4+

``` source
func export(partIDs: [AssignedWorkDocument.PartID]) async throws -> [AssignedWorkDocument.PartID : URL]
```

Deprecated

Use exportParts(identifiedBy:)

## Parameters 

`partIDs`  

An array of part IDs to export. This is treated as a set.

## Return Value

A dictionary of part ID to URLs of the data for the requested parts.

