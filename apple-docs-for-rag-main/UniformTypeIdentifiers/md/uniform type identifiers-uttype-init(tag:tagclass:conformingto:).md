

- Uniform Type Identifiers
- UTType
-  init(tag:tagClass:conformingTo:) 

Initializer

# init(tag:tagClass:conformingTo:)

Creates a type based on a tag, a tag class, and a supertype that it conforms to.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init?(
    tag: String,
    tagClass: UTTagClass,
    conformingTo supertype: UTType?
)
```

## Parameters 

`tag`  

The tag, such as a filename extension.

`tagClass`  

The tag class, such as UTTagClassFilenameExtension.

`supertype`  

Another type that the resulting type must conform to; for example, UTTypeData.

## Discussion

This initializer returns `nil` if the system doesn’t know the tag.

## See Also

### Creating a type

init?(String)

Creates a type based on an identifier.

init?(mimeType: String, conformingTo: UTType)

Creates a type based on a MIME type and a supertype that it conforms to.

init?(filenameExtension: String, conformingTo: UTType)

Creates a type based on a filename extension and an existing supertype that it conforms to.

init(exportedAs: String, conformingTo: UTType?)

Creates a type your app owns based on an identifier and a supertype that it conforms to.

init(importedAs: String, conformingTo: UTType?)

Creates a type your app uses, but doesn’t own, based on an identifier and a supertype that it conforms to.

