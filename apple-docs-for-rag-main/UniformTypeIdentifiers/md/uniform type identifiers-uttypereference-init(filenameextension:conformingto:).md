

- Uniform Type Identifiers
- UTTypeReference
-  init(filenameExtension:conformingTo:) 

Initializer

# init(filenameExtension:conformingTo:)

Creates a type that represents the specified filename extension and conforms to an existing type.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
convenience init?(
    filenameExtension: String,
    conformingTo supertype: UTType
)
```

## Parameters 

`filenameExtension`  

The filename extension.

`supertype`  

The type the resulting type must conform to, such as data or package.

## Discussion

If the system recognizes the filename extension, the intializer returns the corresponding type; otherwise, the initializer returns a dynamic type whose isDeclared and isPublic properties are both set to false.

## See Also

### Creating a type

convenience init?(String)

Creates a type based on an identifier.

convenience init?(mimeType: String)

Creates a type based on a MIME type.

convenience init?(mimeType: String, conformingTo: UTType)

Creates a type based on a MIME type and a supertype that it conforms to.

convenience init?(filenameExtension: String)

Creates a type that represents the specified filename extension.

convenience init?(tag: String, tagClass: String, conformingToType: UTType?)

Creates a type that represents the specified tag and tag class and which conforms to an existing type.

init(exportedAs: String)

Creates a type your app owns based on an identifier.

init(exportedAs: String, conformingTo: UTType)

Creates a type your app owns based on an identifier and a supertype that it conforms to.

init(importedAs: String)

Creates a type your app uses, but doesn’t own, based on an identifier.

init(importedAs: String, conformingTo: UTType)

Creates a type your app uses, but doesn’t own, based on an identifier and a supertype that it conforms to.

