

- Foundation
- AttributedStringAttributeMutation
-  replaceAttributes(\_:with:) 

Instance Method

# replaceAttributes(\_:with:)

Replaces the attributed string’s attributes with those in a specified attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func replaceAttributes(
    _ attributes: AttributeContainer,
    with others: AttributeContainer
)
```

**Required**

## Parameters 

`attributes`  

The existing attributes to replace.

`others`  

The new attributes to apply.

## See Also

### Mutating the String’s Attributes

func setAttributes(AttributeContainer)

Sets the attributed string’s attributes to those in a specified attribute container.

**Required**

func mergeAttributes(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy)

Merges the attributed string’s attributes with those in a specified attribute container.

**Required**

