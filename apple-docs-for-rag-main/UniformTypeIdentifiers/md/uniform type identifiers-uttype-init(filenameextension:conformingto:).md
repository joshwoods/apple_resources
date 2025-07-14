

- Uniform Type Identifiers
- UTType
-  init(filenameExtension:conformingTo:) 

Initializer

# init(filenameExtension:conformingTo:)

Creates a type based on a filename extension and an existing supertype that it conforms to.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init?(
    filenameExtension: String,
    conformingTo supertype: UTType = .data
)
```

## Parameters 

`filenameExtension`  

The filename extension.

`supertype`  

Another type that the resulting type must conform to; for example, UTTypeData or UTTypePackage.

## Discussion

If the system finds no types with the provided filename extension and conformance, but the inputs are otherwise valid, it may provide a dynamic type. The initializer returns `nil` if the parameters aren’t valid.

This initializer is equivalent to calling:

```
UTType(tag: filenameExtension,
       tagClass: .filenameExtension,
       conformingTo: supertype)
```

To get the type of a file on disk, use contentType.

Important

You can’t always derive the type of a file system item based solely on its filename extension.

A type depends on other attributes in addition to the filename extension, including whether the item is a directory.

## See Also

### Creating a type

init?(String)

Creates a type based on an identifier.

init?(mimeType: String, conformingTo: UTType)

Creates a type based on a MIME type and a supertype that it conforms to.

init?(tag: String, tagClass: UTTagClass, conformingTo: UTType?)

Creates a type based on a tag, a tag class, and a supertype that it conforms to.

init(exportedAs: String, conformingTo: UTType?)

Creates a type your app owns based on an identifier and a supertype that it conforms to.

init(importedAs: String, conformingTo: UTType?)

Creates a type your app uses, but doesn’t own, based on an identifier and a supertype that it conforms to.

