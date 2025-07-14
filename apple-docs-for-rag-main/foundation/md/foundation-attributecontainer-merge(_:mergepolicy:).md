

- Foundation
- AttributeContainer
-  merge(\_:mergePolicy:) 

Instance Method

# merge(\_:mergePolicy:)

Merges the container’s attributes with those in another attribute container.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
mutating func merge(
    _ other: AttributeContainer,
    mergePolicy: AttributedString.AttributeMergePolicy = .keepNew
)
```

## Parameters 

`other`  

The attribute container with the attributes to merge.

`mergePolicy`  

A policy to use when resolving conflicts between this string’s attributes and those in `other`.

## See Also

### Modifying Attributes

func merging(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy) -> AttributeContainer

Returns an attribute container by merging the container’s attributes with those in another attribute container.

enum AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

