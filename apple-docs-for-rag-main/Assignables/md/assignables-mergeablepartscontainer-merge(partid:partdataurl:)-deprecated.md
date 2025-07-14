

- Assignables
- MergeablePartsContainer
-  merge(partID:partDataURL:) Deprecated

Instance Method

# merge(partID:partDataURL:)

Merges an individual part into the specified part of this object.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
mutating func merge(
    partID: Self.PartID,
    partDataURL: URL
) throws -> Bool
```

**Required**

Deprecated

Use merge(partData:into:)

## Parameters 

`partID`  

The part ID to merge in.

`partDataURL`  

The URL to the part data file to merge in.

