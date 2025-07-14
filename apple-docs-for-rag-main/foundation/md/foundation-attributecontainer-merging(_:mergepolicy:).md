

- Foundation
- AttributeContainer
-  merging(\_:mergePolicy:) 

Instance Method

# merging(\_:mergePolicy:)

Returns an attribute container by merging the container’s attributes with those in another attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func merging(
    _ other: AttributeContainer,
    mergePolicy: AttributedString.AttributeMergePolicy = .keepNew
) -> AttributeContainer
```

## Parameters 

`other`  

The attribute container with the attributes to merge.

`mergePolicy`  

A policy to use when resolving conflicts between this string’s attributes and those in `other`.

## Return Value

An attribute container created by merging the source container’s attributes with those in another attribute container.

## See Also

### Modifying Attributes

func merge(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy)

Merges the container’s attributes with those in another attribute container.

enum AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

