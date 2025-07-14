

- Foundation
- AttributedString
-  AttributedString.AttributeMergePolicy 

Enumeration

# AttributedString.AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum AttributeMergePolicy
```

## Overview

Use an AttributedString.AttributeMergePolicy when working with methods like `AttributedString/mergeAttributes(_:mergePolicy:)` to indicate how to resolve conflicts between multiple sets of attributes. When a source string and a merging attribute container both contain a given attribute with different values, the merge policy determines how to resolve the conflict.

## Topics

### Merge Policies

case keepCurrent

A policy to keep the string’s current attribute value when merging multiple sets of attributes.

case keepNew

A policy to keep the newly-merged attribute value when merging multiple sets of attributes.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Applying and Modifying Attributes

protocol AttributedStringAttributeMutation

A protocol that defines in-place mutations for attributes in an attributed string.

