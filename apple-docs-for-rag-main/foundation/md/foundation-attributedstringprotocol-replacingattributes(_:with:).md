

- Foundation
- AttributedStringProtocol
-  replacingAttributes(\_:with:) 

Instance Method

# replacingAttributes(\_:with:)

Returns an attributed string by replacing occurrences of attributes in one attribute container with those in another attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func replacingAttributes(
    _ attributes: AttributeContainer,
    with others: AttributeContainer
) -> AttributedString
```

## Parameters 

`attributes`  

The existing attributes to replace.

`others`  

The new attributes to apply.

## Return Value

An attributed string created by replacing occurrences of attributes in one attribute container with those in another attribute container.

## See Also

### Applying Attributes

func settingAttributes(AttributeContainer) -> AttributedString

Returns an attributed string by setting the attributed string’s attributes to those in a specified attribute container.

func mergingAttributes(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy) -> AttributedString

Returns an attributed string by merging the attributed string’s attributes with those in a specified attribute container.

enum AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

