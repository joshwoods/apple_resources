

- Foundation
- AttributedStringAttributeMutation
-  setAttributes(\_:) 

Instance Method

# setAttributes(\_:)

Sets the attributed string’s attributes to those in a specified attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func setAttributes(_ attributes: AttributeContainer)
```

**Required**

## Parameters 

`attributes`  

The attribute container with the attributes to apply.

## See Also

### Mutating the String’s Attributes

func mergeAttributes(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy)

Merges the attributed string’s attributes with those in a specified attribute container.

**Required**

func replaceAttributes(AttributeContainer, with: AttributeContainer)

Replaces the attributed string’s attributes with those in a specified attribute container.

**Required**

