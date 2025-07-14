

- Foundation
-  AttributeContainer 

Structure

# AttributeContainer

A container for attribute keys and values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@dynamicMemberLookup
struct AttributeContainer
```

## Overview

AttributeContainer provides a way to store attributes and their values outside of an attributed string. You use this type to initialize an instance of AttributedString with preset attributes, and to set, merge, or replace attributes in existing attributed strings.

## Topics

### Creating an Attribute Container

init()

Creates an empty attribute container.

init&lt;S>([NSAttributedString.Key : Any], including: S.Type) throws

Creates an attribute container from a dictionary and an attribute scope.

init&lt;S>([NSAttributedString.Key : Any], including: KeyPath&lt;AttributeScopes, S.Type>) throws

Creates an attribute container from a dictionary and an attribute scope that a key path identifies.

init([NSAttributedString.Key : Any])

Creates an attribute container from a dictionary, using default attribute scopes.

### Accessing Attributes

subscript&lt;T>(T.Type) -> T.Value?

Returns the attribute that corresponds to a specified key.

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> K.Value?

Returns the attribute that corresponds to a specified key path.

subscript&lt;S>(dynamicMember _: KeyPath&lt;AttributeScopes, S.Type>) -> ScopedAttributeContainer&lt;S>

Returns the attribute container that corresponds to a specified key path.

subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> AttributeContainer.Builder&lt;K>

Returns a modified attribute container as part of building a chain of attributes.

static subscript&lt;K>(dynamicMember _: KeyPath&lt;AttributeDynamicLookup, K>) -> AttributeContainer.Builder&lt;K>

Returns a modified attribute container as part of building a chain of attributes, for use as a static method.

protocol AttributedStringKey

A type that defines an attribute’s name and type.

struct Builder

A type that iteratively builds attribute containers by setting attribute values.

### Modifying Attributes

func merge(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy)

Merges the container’s attributes with those in another attribute container.

func merging(AttributeContainer, mergePolicy: AttributedString.AttributeMergePolicy) -> AttributeContainer

Returns an attribute container by merging the container’s attributes with those in another attribute container.

enum AttributeMergePolicy

An enumeration of behaviors to apply when merging attributes.

### Interoperating with Objective-C Attributes

protocol ObjectiveCConvertibleAttributedStringKey

A protocol that defines Objective-C interoperability with an attribute key’s value type.

## Relationships

### Conforms To

- Copyable
- CustomStringConvertible
- DecodableWithConfiguration
- EncodableWithConfiguration
- Equatable
- Hashable
- Sendable

## See Also

### Creating an Attributed String

init()

Creates an empty attributed string.

init(AttributedSubstring)

Creates an attributed string from an attributed substring.

init(String, attributes: AttributeContainer)

Creates an attributed string from a string and an attribute container.

init(Substring, attributes: AttributeContainer)

Creates an attributed string from a substring and an attribute container.

init&lt;S>(S, attributes: AttributeContainer)

Creates an attributed string from a character sequence and an attribute container.

