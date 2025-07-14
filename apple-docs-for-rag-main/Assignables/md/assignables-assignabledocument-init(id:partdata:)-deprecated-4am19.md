

- Assignables
- AssignableDocument
-  init(id:partData:) Deprecated

Initializer

# init(id:partData:)

Construct an instance of this object with the parts data passed in.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS

``` source
init(
    id: AssignableDocument.ID,
    partData: [AssignableDocument.PartID : URL]
) throws
```

Deprecated

Use async init(id:partData:)

## Parameters 

`id`  

The ID of this document.

`partData`  

A dictionary of part IDs to `URL` objects that contain the serialized parts data.

