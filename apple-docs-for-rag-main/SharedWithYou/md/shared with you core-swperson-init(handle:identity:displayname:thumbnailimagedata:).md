

- Shared With You Core
- SWPerson
-  init(handle:identity:displayName:thumbnailImageData:) 

Initializer

# init(handle:identity:displayName:thumbnailImageData:)

Creates and initializes a person object.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
init(
    handle: String?,
    identity: SWPerson.Identity?,
    displayName: String,
    thumbnailImageData: Data?
)
```

## Parameters 

`handle`  

The phone number or email address for this person.

`identity`  

The identity of this person.

`displayName`  

The name of this person.

`thumbnailImageData`  

The thumbnail image data for this person. If `nil`, this will be inferred by the system.

