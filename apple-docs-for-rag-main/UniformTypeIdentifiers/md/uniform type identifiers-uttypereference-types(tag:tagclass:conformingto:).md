

- Uniform Type Identifiers
- UTTypeReference
-  types(tag:tagClass:conformingTo:) 

Type Method

# types(tag:tagClass:conformingTo:)

Returns an array of types from the provided tag and tag class.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class func types(
    tag: String,
    tagClass: String,
    conformingTo supertype: UTType?
) -> [UTType]
```

## Parameters 

`tag`  

The desired tag, such as a filename extension.

`tagClass`  

The tag class, such as UTTagClassFilenameExtension.

`supertype`  

Another type that the resulting type must conform to; for example, UTTypeData.

