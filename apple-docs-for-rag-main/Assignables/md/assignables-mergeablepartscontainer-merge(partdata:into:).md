

- Assignables
- MergeablePartsContainer
-  merge(partData:into:) 

Instance Method

# merge(partData:into:)

Merges an individual part into the specified part of this object.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+visionOS

``` source
mutating func merge(
    partData: MergeablePartData,
    into partID: Self.PartID
) async throws -> Bool
```

**Required**

## Parameters 

`partData`  

The part data to merge into this object.

`partID`  

The part ID of the part that the incoming data should be merged in.

## Return Value

`true`, if the merge caused a mutation.

