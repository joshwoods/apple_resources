

- Uniform Type Identifiers
- UTType
-  init(exportedAs:conformingTo:) 

Initializer

# init(exportedAs:conformingTo:)

Creates a type your app owns based on an identifier and a supertype that it conforms to.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
init(
    exportedAs identifier: String,
    conformingTo parentType: UTType? = nil
)
```

## Parameters 

`identifier`  

The identifier of your type.

`parentType`  

A type to extend for your own type.

## Discussion

Defining a type with this initializer asserts that you own the type definition. For example, you might define your file format in code to use it to save or open files in your app.

```
```

## See Also

### Creating a type

init?(String)

Creates a type based on an identifier.

init?(mimeType: String, conformingTo: UTType)

Creates a type based on a MIME type and a supertype that it conforms to.

init?(filenameExtension: String, conformingTo: UTType)

Creates a type based on a filename extension and an existing supertype that it conforms to.

init?(tag: String, tagClass: UTTagClass, conformingTo: UTType?)

Creates a type based on a tag, a tag class, and a supertype that it conforms to.

init(importedAs: String, conformingTo: UTType?)

Creates a type your app uses, but doesn’t own, based on an identifier and a supertype that it conforms to.

