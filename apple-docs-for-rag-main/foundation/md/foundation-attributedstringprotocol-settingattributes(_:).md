

- Foundation
- AttributedStringProtocol
-  settingAttributes(\_:) 

Instance Method

# settingAttributes(\_:)

Returns an attributed string by setting the attributed string’s attributes to those in a specified attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func settingAttributes(_ attributes: AttributeContainer) -> AttributedString
```

## Parameters 

`attributes`  

The attribute container with the attributes to apply.

## Return Value

An attributed string from setting the attributed string’s attributes to those in a specified attribute container.

## See Also

### Applying Attributes

func mergingAttributes(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy) -> AttributedString

Returns an attributed string by merging the attributed string’s attributes with those in a specified attribute container.

enum AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

func replacingAttributes(AttributeContainer, with: AttributeContainer) -> AttributedString

Returns an attributed string by replacing occurrences of attributes in one attribute container with those in another attribute container.

