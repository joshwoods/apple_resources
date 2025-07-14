

- Assignables
- AssignedWorkDocument
-  init(id:assignableDocument:partData:) Deprecated

Initializer

# init(id:assignableDocument:partData:)

Construct an instance of this object with the parts data passed in.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
init(
    id: AssignedWorkDocument.ID,
    assignableDocument: AssignableDocument,
    partData: [AssignedWorkDocument.PartID : URL]
) throws
```

Deprecated

Use async init(id:assignableDocument:partData:)

## Parameters 

`id`  

The ID of the document.

`assignableDocument`  

The assignable document that this work document is based on.

`partData`  

A dictionary of part ID to URLs of the data stored on disk for the requested parts.

