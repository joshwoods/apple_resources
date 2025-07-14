

- Assignables
- AssignableDocument
-  merge(partID:partDataURL:) Deprecated

Instance Method

# merge(partID:partDataURL:)

Merges an individual part’s data into the specified part of this object.

iOS 17.4+iPadOS 17.4+visionOSMac Catalyst 17.4+

``` source
@discardableResult
mutating func merge(
    partID: AssignableDocument.PartID,
    partDataURL: URL
) throws -> Bool
```

Deprecated

Use merge(partData:into:)

## Parameters 

`partID`  

The part ID to merge in.

`partDataURL`  

The URL to the part data to merge in.

