

- Foundation
- AttributedStringProtocol
-  mergingAttributes(\_:mergePolicy:) 

Instance Method

# mergingAttributes(\_:mergePolicy:)

Returns an attributed string by merging the attributed string’s attributes with those in a specified attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func mergingAttributes(
    _ attributes: AttributeContainer,
    mergePolicy: AttributedString.AttributeMergePolicy = .keepNew
) -> AttributedString
```

## Parameters 

`attributes`  

The attribute container with the attributes to merge.

`mergePolicy`  

A policy to use when resolving conflicts between this string’s attributes and those in `attributes`.

## Return Value

An attributed string from merging the attributed string’s attributes with those in a specified attribute container. In cases where the same attribute exists in both the source string and `attributes`, the `mergePolicy` determines which value the returned string uses.

## See Also

### Applying Attributes

func settingAttributes(AttributeContainer) -> AttributedString

Returns an attributed string by setting the attributed string’s attributes to those in a specified attribute container.

enum AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

func replacingAttributes(AttributeContainer, with: AttributeContainer) -> AttributedString

Returns an attributed string by replacing occurrences of attributes in one attribute container with those in another attribute container.

