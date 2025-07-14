

- Foundation
-  AttributedStringAttributeMutation 

Protocol

# AttributedStringAttributeMutation

A protocol that defines in-place mutations for attributes in an attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol AttributedStringAttributeMutation
```

## Topics

### Mutating the String’s Attributes

func setAttributes(AttributeContainer)

Sets the attributed string’s attributes to those in a specified attribute container.

**Required**

func mergeAttributes(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy)

Merges the attributed string’s attributes with those in a specified attribute container.

**Required**

func replaceAttributes(AttributeContainer, with: AttributeContainer)

Replaces the attributed string’s attributes with those in a specified attribute container.

**Required**

## Relationships

### Inherited By

- AttributedStringProtocol

### Conforming Types

- AttributedString
- AttributedSubstring

## See Also

### Applying and Modifying Attributes

enum AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

