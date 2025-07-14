

- Foundation
- AttributeContainer
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Returns the attribute that corresponds to a specified key.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency
subscript(_: T.Type) -> T.Value? where T : AttributedStringKey, T.Value : Sendable { get set }
```

## See Also

### Accessing Attributes

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

