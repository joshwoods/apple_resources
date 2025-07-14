

- Assignables
- MergeablePartsContainer
-  makePart(for:) 

Instance Method

# makePart(for:)

Creates data for the part with the given identifier.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS

``` source
func makePart(for partID: Self.PartID) throws -> MergeablePartData?
```

**Required**

## Parameters 

`partID`  

The identifier for the part you want to create.

## Return Value

Part data for the `partID` provided, if possible. Otherwise, `nil`.

## Discussion

In cases where this document is a partial one, i.e. it is missing some parts, you use this method to create data for the missing part. You then use merge(partData:into:) to merge the newly created data into this document.

