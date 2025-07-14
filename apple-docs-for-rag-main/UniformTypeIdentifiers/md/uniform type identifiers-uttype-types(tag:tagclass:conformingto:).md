

- Uniform Type Identifiers
- UTType
-  types(tag:tagClass:conformingTo:) 

Type Method

# types(tag:tagClass:conformingTo:)

Returns an array of types from the provided tag and tag class.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static func types(
    tag: String,
    tagClass: UTTagClass,
    conformingTo supertype: UTType?
) -> [UTType]
```

## Parameters 

`tag`  

The tag, such as a filename extension.

`tagClass`  

The tag class, such as filenameExtension.

`supertype`  

Another type to which resulting types must conform. A value of `nil` indicates that conformance isn’t required.

## Discussion

If the system doesn’t find any types with the provided tag but the inputs were otherwise valid, it may provide a dynamic type. The initializer returns an empty array if the inputs aren’t valid.

