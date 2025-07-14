

- Foundation
- AttributedStringAttributeMutation
-  mergeAttributes(\_:mergePolicy:) 

Instance Method

# mergeAttributes(\_:mergePolicy:)

Merges the attributed string’s attributes with those in a specified attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func mergeAttributes(
    _ attributes: AttributeContainer,
    mergePolicy: AttributedString.AttributeMergePolicy
)
```

**Required**

## Parameters 

`attributes`  

The attribute container with the attributes to merge.

`mergePolicy`  

A policy to use when resolving conflicts between this string’s attributes and those in `attributes`.

## See Also

### Mutating the String’s Attributes

func setAttributes(AttributeContainer)

Sets the attributed string’s attributes to those in a specified attribute container.

**Required**

func replaceAttributes(AttributeContainer, with: AttributeContainer)

Replaces the attributed string’s attributes with those in a specified attribute container.

**Required**

