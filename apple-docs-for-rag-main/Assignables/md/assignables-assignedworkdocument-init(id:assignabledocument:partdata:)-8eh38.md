

- Assignables
- AssignedWorkDocument
-  init(id:assignableDocument:partData:) 

Initializer

# init(id:assignableDocument:partData:)

Construct an instance of this object with the parts data passed in.

iOS 17.5+iPadOS 17.5+Mac Catalyst 17.5+visionOS

``` source
init(
    id: AssignedWorkDocument.ID,
    assignableDocument: AssignableDocument,
    partData: [AssignedWorkDocument.PartID : MergeablePartData]
) async throws
```

## Parameters 

`id`  

The ID of this document.

`partData`  

A dictionary of part IDs to MergeablePartData objects that contain the parts data.

