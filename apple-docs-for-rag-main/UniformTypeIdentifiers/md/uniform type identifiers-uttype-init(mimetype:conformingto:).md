

- Uniform Type Identifiers
- UTType
-  init(mimeType:conformingTo:) 

Initializer

# init(mimeType:conformingTo:)

Creates a type based on a MIME type and a supertype that it conforms to.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init?(
    mimeType: String,
    conformingTo supertype: UTType = .data
)
```

## Parameters 

`mimeType`  

A string that represents the MIME type.

`supertype`  

Another UTType instance that the resulting type must conform to; for example, UTTypeData.

## Discussion

This initializer is equivalent to calling:

```
UTType(tag: mimeType,
       tagClass: .mimeType,
       conformingTo: supertype)
```

The initializer may provide a dynamic type if the parameters are valid, but the system doesn’t find any types with the MIME type and conformance. The initializer returns `nil` if the parameters aren’t valid.

## See Also

### Creating a type

init?(String)

Creates a type based on an identifier.

init?(filenameExtension: String, conformingTo: UTType)

Creates a type based on a filename extension and an existing supertype that it conforms to.

init?(tag: String, tagClass: UTTagClass, conformingTo: UTType?)

Creates a type based on a tag, a tag class, and a supertype that it conforms to.

init(exportedAs: String, conformingTo: UTType?)

Creates a type your app owns based on an identifier and a supertype that it conforms to.

init(importedAs: String, conformingTo: UTType?)

Creates a type your app uses, but doesn’t own, based on an identifier and a supertype that it conforms to.

