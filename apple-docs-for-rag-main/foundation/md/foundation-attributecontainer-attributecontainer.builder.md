

- Foundation
- AttributeContainer
-  AttributeContainer.Builder 

Structure

# AttributeContainer.Builder

A type that iteratively builds attribute containers by setting attribute values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Builder where T : AttributedStringKey
```

## Overview

The AttributeContainer.Builder type lets you build AttributeContainer instances by chaining together several attributes in one expression. The following example shows this approach:

```
// An attribute container with the link and backgroundColor attributes.
let myContainer = AttributeContainer().link(myURL).backgroundColor(.yellow)
```

The first part of this expression, `AttributeContainer().link(URL(myURL))`, creates a builder to apply the link attribute to the empty AttributeContainer. The builder’s callAsFunction(_:) returns a new AttributeContainer with this attribute set. Then the `backgroundColor(.yellow)` creates a second builder to modify the just-returned AttributeContainer by adding the backgroundColor attribute. The result is an AttributeContainer with both attributes set.

## Topics

### Calling Builder Functions

func callAsFunction(T.Value) -> AttributeContainer

Builds an attribute container by setting an attribute and returning a modified attribute container.

## Relationships

### Conforms To

- Sendable

## See Also

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

